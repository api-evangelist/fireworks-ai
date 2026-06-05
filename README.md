# Fireworks AI (fireworks-ai)

Fireworks AI is a production-grade inference platform for open-source and proprietary generative models. The Fireworks API hosts Llama, DeepSeek, Qwen, Mixtral, Stable Diffusion, and other models with serverless pay-per-token, on-demand dedicated GPU, and batch deployment options, plus managed fine-tuning.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/fireworks-ai/refs/heads/main/apis.yml)

## Tags

- AI
- LLM
- Inference
- Multimodal
- Fine-tuning
- GPU

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-29

## APIs

### Fireworks Chat Completions API

OpenAI-compatible chat completions across 100+ open-source and proprietary models including Llama, DeepSeek, Qwen, and Mixtral, with streaming, function calling, and structured outputs.

- **Human URL:** [https://docs.fireworks.ai/api-reference/post-chatcompletions](https://docs.fireworks.ai/api-reference/post-chatcompletions)
- **Base URL:** `https://api.fireworks.ai/inference/v1`

#### Tags

- Chat
- Completions
- LLM

#### Properties

- [Documentation](https://docs.fireworks.ai/guides/querying-text-models)
- [API Reference](https://docs.fireworks.ai/api-reference/post-chatcompletions)
- [OpenAPI](openapi/fireworks-ai-merged-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireworks-ai-merged.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireworks-ai-merged.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/fireworks-ai-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Fireworks Completions API

Legacy text completion endpoint, OpenAI-compatible.

- **Human URL:** [https://docs.fireworks.ai/api-reference/post-completions](https://docs.fireworks.ai/api-reference/post-completions)
- **Base URL:** `https://api.fireworks.ai/inference/v1`

#### Tags

- Completions
- LLM

#### Properties

- [API Reference](https://docs.fireworks.ai/api-reference/post-completions)
- [OpenAPI](openapi/fireworks-ai-merged-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireworks-ai-merged.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireworks-ai-merged.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/fireworks-ai-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Fireworks Vision API

Vision-language inference for image and document understanding through chat completions.

- **Human URL:** [https://docs.fireworks.ai/guides/querying-vision-language-models](https://docs.fireworks.ai/guides/querying-vision-language-models)
- **Base URL:** `https://api.fireworks.ai/inference/v1`

#### Tags

- Vision
- Multimodal
- Documents

#### Properties

- [Documentation](https://docs.fireworks.ai/guides/querying-vision-language-models)
- [OpenAPI](openapi/fireworks-ai-merged-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireworks-ai-merged.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireworks-ai-merged.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fireworks Embeddings API

Generate dense vector embeddings for retrieval, RAG, and semantic search using nomic, Qwen3, BGE, and other open embedding models.

- **Human URL:** [https://docs.fireworks.ai/guides/querying-embeddings-models](https://docs.fireworks.ai/guides/querying-embeddings-models)
- **Base URL:** `https://api.fireworks.ai/inference/v1`

#### Tags

- Embeddings
- Vector
- Retrieval

#### Properties

- [Documentation](https://docs.fireworks.ai/guides/querying-embeddings-models)
- [OpenAPI](openapi/fireworks-ai-merged-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireworks-ai-merged.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireworks-ai-merged.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fireworks Rerank API

Cross-encoder reranking of candidate passages for higher-quality retrieval and RAG pipelines.

- **Human URL:** [https://docs.fireworks.ai/guides/querying-rerank-models](https://docs.fireworks.ai/guides/querying-rerank-models)
- **Base URL:** `https://api.fireworks.ai/inference/v1`

#### Tags

- Rerank
- Retrieval
- RAG

#### Properties

- [Documentation](https://docs.fireworks.ai/guides/querying-rerank-models)
- [OpenAPI](openapi/fireworks-ai-merged-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireworks-ai-merged.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireworks-ai-merged.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fireworks Images API

Text-to-image and image-to-image generation across Stable Diffusion, FLUX, and other diffusion model families.

- **Human URL:** [https://docs.fireworks.ai/api-reference/generate-a-new-image-from-a-text-prompt](https://docs.fireworks.ai/api-reference/generate-a-new-image-from-a-text-prompt)
- **Base URL:** `https://api.fireworks.ai/inference/v1`

#### Tags

- Images
- Generation
- Stable Diffusion

#### Properties

- [Documentation](https://docs.fireworks.ai/guides/querying-image-language-models)
- [API Reference](https://docs.fireworks.ai/api-reference/generate-a-new-image-from-a-text-prompt)
- [OpenAPI](openapi/fireworks-ai-merged-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireworks-ai-merged.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireworks-ai-merged.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fireworks Audio API

OpenAI-compatible audio transcription, translation, and TTS endpoints for Whisper and other audio models with low-latency streaming.

- **Human URL:** [https://docs.fireworks.ai/api-reference/audio-transcriptions](https://docs.fireworks.ai/api-reference/audio-transcriptions)
- **Base URL:** `https://audio-prod.us-virginia-1.direct.fireworks.ai/v1`

#### Tags

- Audio
- Speech to Text
- Text to Speech
- Whisper

#### Properties

- [Documentation](https://docs.fireworks.ai/guides/audio)
- [API Reference](https://docs.fireworks.ai/api-reference/audio-transcriptions)
- [OpenAPI](openapi/fireworks-ai-merged-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireworks-ai-merged.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireworks-ai-merged.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fireworks Batch Inference API

Asynchronous batch inference at 50% of serverless rates for both input and output tokens.

- **Human URL:** [https://docs.fireworks.ai/guides/batch-inference](https://docs.fireworks.ai/guides/batch-inference)
- **Base URL:** `https://api.fireworks.ai/inference/v1`

#### Tags

- Batch
- Async

#### Properties

- [Documentation](https://docs.fireworks.ai/guides/batch-inference)
- [OpenAPI](openapi/fireworks-ai-merged-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireworks-ai-merged.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireworks-ai-merged.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fireworks Fine-Tuning API

Supervised fine-tuning (LoRA and full-parameter) and reinforcement fine-tuning, with one-click deployment of fine-tuned weights at the same per-token price as base models.

- **Human URL:** [https://docs.fireworks.ai/fine-tuning/fine-tuning-models](https://docs.fireworks.ai/fine-tuning/fine-tuning-models)
- **Base URL:** `https://api.fireworks.ai/v1`

#### Tags

- Fine-Tuning
- LoRA
- RFT
- Training

#### Properties

- [Documentation](https://docs.fireworks.ai/fine-tuning/fine-tuning-models)
- [OpenAPI](openapi/fireworks-ai-merged-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireworks-ai-merged.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireworks-ai-merged.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fireworks Files API

Upload and manage training datasets, batch input files, and fine-tuning artifacts.

- **Human URL:** [https://docs.fireworks.ai/api-reference/files](https://docs.fireworks.ai/api-reference/files)
- **Base URL:** `https://api.fireworks.ai/v1`

#### Tags

- Files
- Datasets

#### Properties

- [API Reference](https://docs.fireworks.ai/api-reference/files)
- [OpenAPI](openapi/fireworks-ai-merged-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireworks-ai-merged.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireworks-ai-merged.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fireworks Models API

Lists models, deployments, and metadata across the Fireworks catalog.

- **Human URL:** [https://docs.fireworks.ai/api-reference/list-models](https://docs.fireworks.ai/api-reference/list-models)
- **Base URL:** `https://api.fireworks.ai/v1`

#### Tags

- Models
- Catalog

#### Properties

- [API Reference](https://docs.fireworks.ai/api-reference/list-models)
- [OpenAPI](openapi/fireworks-ai-merged-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireworks-ai-merged.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireworks-ai-merged.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fireworks Deployments API

Provision and autoscale on-demand dedicated GPU deployments (H100, H200, B200, B300) billed per GPU-second.

- **Human URL:** [https://docs.fireworks.ai/guides/ondemand-deployments](https://docs.fireworks.ai/guides/ondemand-deployments)
- **Base URL:** `https://api.fireworks.ai/v1`

#### Tags

- Deployments
- On-Demand
- GPU

#### Properties

- [Documentation](https://docs.fireworks.ai/guides/ondemand-deployments)
- [OpenAPI](openapi/fireworks-ai-merged-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireworks-ai-merged.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireworks-ai-merged.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fireworks Account API

Programmatic access to account, billing, usage, and team management.

- **Human URL:** [https://docs.fireworks.ai/api-reference](https://docs.fireworks.ai/api-reference)
- **Base URL:** `https://api.fireworks.ai/v1`

#### Tags

- Account
- Usage
- Billing

#### Properties

- [API Reference](https://docs.fireworks.ai/api-reference)
- [OpenAPI](openapi/fireworks-ai-merged-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireworks-ai-merged.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireworks-ai-merged.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/fw-ai)
- [LinkedIn](https://www.linkedin.com/company/fireworks-ai)
- [Website](https://fireworks.ai/)
- [Documentation](https://docs.fireworks.ai/)
- [Plans](plans/fireworks-ai-plans-pricing.yml)
- [Rate Limits](rate-limits/fireworks-ai-rate-limits.yml)
- [Fin Ops](finops/fireworks-ai-finops.yml)
- [Integrations](https://fireworks.ai/partners)
- [L L Ms Txt](https://docs.fireworks.ai/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
