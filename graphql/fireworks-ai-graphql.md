# Fireworks AI GraphQL Schema

This directory contains a conceptual GraphQL schema for the Fireworks AI fast inference platform. The schema is derived from the public Fireworks AI REST API surface documented at https://docs.fireworks.ai/ and represents the same capabilities in GraphQL vocabulary.

## Provider

**Name:** Fireworks AI
**Website:** https://fireworks.ai/
**API Docs:** https://docs.fireworks.ai/
**Base URL:** https://api.fireworks.ai/inference/v1

## Schema File

- `fireworks-ai-schema.graphql` — Full conceptual GraphQL schema (60+ named types)

## Coverage

The schema covers all major Fireworks AI API surface areas:

### Models
- `Model` — catalog entry with type, provider, capabilities, and context length
- `ModelDetails` — architecture, parameter count, quantization, license, HuggingFace ID
- `ModelType` — CHAT, COMPLETION, EMBEDDING, RERANK, IMAGE, AUDIO, REASONING, MULTIMODAL
- `ModelProvider` — Meta, Mistral, Qwen, DeepSeek, Stability AI, Black Forest Labs, Fireworks, Community
- `ModelCapability` — TEXT_GENERATION, FUNCTION_CALLING, STRUCTURED_OUTPUT, VISION, etc.
- `ModelConfig` — temperature, top-p, top-k, max tokens, stop sequences, seed

### Deployments
- `Deployment` — on-demand dedicated GPU deployment with status lifecycle
- `DeploymentDetails` — GPU type (H100/H200/B200/B300), region, replica counts, inference URL, cost-per-GPU-second
- `DeploymentStatus` — PENDING, INITIALIZING, RUNNING, SCALING, PAUSED, STOPPED, FAILED, DELETING
- `DeploymentConfig` — auto-scale, scale-to-zero, idle timeout, LoRA adapters

### Chat Completions
- `ChatCompletion` — top-level response with choices, usage, and system fingerprint
- `ChatMessage` — role-tagged message with optional tool calls and refusal field
- `ChatRole` — SYSTEM, USER, ASSISTANT, TOOL, FUNCTION
- `ChatCompletionChoice` — individual generation with finish reason and logprobs

### Text Completions
- `CompletionRequest` — legacy /completions endpoint request
- `CompletionDetails` — all sampling parameters
- `CompletionChoice` — text output with logprobs
- `CompletionMessage` — message wrapper with tool call support

### Function Calling / Tools
- `Tool` — name, description, JSON parameters schema, strict mode
- `ToolFunction` — function definition for the tool
- `FunctionCall` — structured call emitted by the model (id, type, function details)
- `ToolChoice` — NONE, AUTO, REQUIRED enum
- `ToolResult` — tool output to feed back in the next turn

### Embeddings
- `EmbeddingRequest` — model, input strings, encoding format, dimensions
- `EmbeddingResult` — list of embedding vectors with usage
- `EmbeddingVector` — index, object type, dense float32 vector

### Audio
- `SpeechToText` — transcription request (Whisper-compatible)
- `AudioTranscription` — text, language, duration, segments, word-level timestamps
- `AudioTranslation` — translation to English with segments
- `AudioSegment` — chunk with start/end, tokens, log-prob, compression ratio
- `AudioWord` — word-level timestamp pair
- `AudioFormat` — MP3, WAV, FLAC, OGG, PCM, OPUS

### Image Generation
- `ImageGeneration` — text-to-image and image-to-image request (FLUX, Stable Diffusion)
- `ImageResult` — list of generated images with seeds
- `GeneratedImage` — URL or base64, seed, revised prompt, dimensions
- `SamplerType` — DDIM, DDPM, Euler, Euler-A, DPM++2M, DPM++SDE
- `ImageFormat` — PNG, JPEG, WEBP

### Reasoning
- `ReasoningModel` — model with thinking budget and streaming thoughts support
- `ReasoningStep` — thought, action, observation with token count

### Fine-Tuning
- `FineTuningJob` — supervised or reinforcement fine-tuning job lifecycle
- `FineTuningStatus` — QUEUED, RUNNING, SUCCEEDED, FAILED, CANCELLED
- `FineTuningDetails` — method (LoRA / full-param / RFT), hyperparameters, estimated cost
- `TrainingFile` — uploaded dataset file with line count and status
- `CheckpointDetails` — step, metrics (train/valid loss and accuracy)
- `CheckpointMetrics` — quantitative training metrics per checkpoint

### Batch Inference
- `BatchJob` — async batch request at 50% serverless discount
- `BatchJobStatus` — VALIDATING, IN_PROGRESS, COMPLETED, FAILED, CANCELLED, EXPIRED
- `BatchDetails` — request counts, token totals, discount percentage, metadata

### Usage and Cost
- `Usage` — account-level usage for a billing period with breakdown by model
- `TokenUsage` — prompt, completion, total, cached, audio, image token counts
- `CostEstimate` — prompt cost, completion cost, GPU cost, storage cost in USD
- `UsageBreakdown` — per-model slice of usage and cost

### Prompts and Templates
- `PromptTemplate` — named template with variable substitution and linked system prompt
- `TemplateVariable` — name, description, default, required flag
- `SystemPrompt` — reusable system message with token count

### Account and Auth
- `Account` — top-level account with plan and API keys
- `AccountDetails` — email, org, credit balance, monthly spend limit
- `AccountPlan` — FREE, GROWTH, SCALE, ENTERPRISE
- `APIKey` — key with prefix, scopes, expiry, last-used timestamp
- `Token` — OAuth-style access token envelope

### Error Handling and Rate Limits
- `Error` — code, message, type, param, details
- `RateLimitInfo` — per-minute request/token limits, remaining counts, reset times, retry-after

## Operations

### Queries (14)
`model`, `models`, `deployment`, `deployments`, `account`, `usage`, `fineTuningJob`, `fineTuningJobs`, `trainingFile`, `trainingFiles`, `batchJob`, `batchJobs`, `apiKeys`, `promptTemplates`

### Mutations (16)
`createCompletion`, `createChatCompletion`, `createEmbedding`, `generateImage`, `transcribeAudio`, `translateAudio`, `createDeployment`, `updateDeployment`, `stopDeployment`, `deleteDeployment`, `createFineTuningJob`, `cancelFineTuningJob`, `uploadTrainingFile`, `deleteTrainingFile`, `createBatchJob`, `cancelBatchJob`

### Subscriptions (5)
`chatCompletionStream`, `completionStream`, `fineTuningJobUpdates`, `batchJobUpdates`, `deploymentStatusUpdates`

## Type Count

63 named types (scalars, enums, object types) plus Query, Mutation, and Subscription root types.

## Related Resources

- OpenAPI spec: `openapi/fireworks-ai-merged-openapi.yml`
- AsyncAPI spec: `asyncapi/fireworks-ai-asyncapi.yml`
- Plans and pricing: `plans/fireworks-ai-plans-pricing.yml`
- Rate limits: `rate-limits/fireworks-ai-rate-limits.yml`
- FinOps: `finops/fireworks-ai-finops.yml`
