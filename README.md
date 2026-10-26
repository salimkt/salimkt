<h1 align="center">Muhammed Salim K T</h1>

<p align="center">
  <strong>AI/ML Engineer: LLM systems, RAG, agent orchestration, speech &amp; vision</strong><br>
  4+ years shipping production AI · Kochi, India<br>
  Open to roles in the UAE/Gulf, Europe (with relocation) and remote
</p>

<p align="center">
  <a href="https://muhammed-salim.onrender.com">Portfolio</a> ·
  <a href="https://www.linkedin.com/in/muhammed-salim-k-t-498125165">LinkedIn</a> ·
  <a href="mailto:mohdsalimkt@gmail.com">mohdsalimkt@gmail.com</a>
</p>

---

I build production LLM systems end to end: agent orchestration, retrieval, speech pipelines, model serving, and the evaluation that keeps them honest. Most of it runs on-premise and air-gapped inside enterprise customers' own infrastructure.

### At a glance

- **12B → 32B-class:** my multi-agent engine lets a 12B model do 32B-class work, moving each deployment from a GPU cluster to a single node
- **10M+ embeddings** in production RAG, serving **10k+ queries/day**
- **+45%** answer accuracy over the bare-LLM baseline, **1.8 s** average inference latency, **99.7%** uptime
- **94%** speech-to-text accuracy and **92%** live-caption accuracy in production
- **50k+ concurrent users** on real-time WebSocket / REST services
- **8 Kubernetes environments**, including **two GPU/DGX clusters**

### What I have built at work

**Multi-agent tool-calling engine.** `bm-agent-engine` replaced the CrewAI-based orchestration of an on-premise enterprise LLM platform and now serves all its agent traffic; I was the largest contributor to its ~49k lines. A 73-toolset registry, ReAct agents with tiered escalation, and a FAST / SMALL / LARGE / THINKING router over vLLM and Ollama. Because the SSE event contract was kept exactly, the UI cut over with a single config change.

**Enterprise RAG.** Docling + RapidOCR ingestion, Sentence-Transformers embeddings, a Cassandra vector schema, and hybrid keyword + semantic retrieval with re-ranking over 10M+ embeddings. Quantization, batching and caching brought average inference to 1.8 s; model failover and warm caching hold 99.7% uptime.

**Speech AI in production.** A transcription service for a US hosted-telephony provider's voicemail and call recordings: NVIDIA Canary and Whisper on vLLM with automatic failover, Redis priority queues and Celery workers, recordings up to 10 hours, and speaker diarization. Also: Whisper STT (94%), Tacotron2 TTS and live captions (92%) in a video-calling product.

**Vision and documents.** PaddleOCR-VL and Qwen-VL served through Transformers, a pluggable OCR layer feeding RAG, and LayoutLMv3 fine-tuned to 91% F1 on 100K+ documents a month.

### Selected public work

| Project | What it is |
|---|---|
| **[DataRat](https://github.com/salimkt/DataRat)** · [live demo](https://salimkt.github.io/DataRat/) | AI data analyst. Connect 11 kinds of data source and get KPIs, anomalies and Holt-Winters forecasts; a Planner → SQL → Analyst → Narrator agent pipeline answers plain-English questions, with a rules engine as fallback and a read-only SQL guard. FastAPI, DuckDB, React. |
| **[3xDezine](https://github.com/salimkt/3xdezine)** · [live demo](https://salimkt.github.io/3xdezine/) | Home design and costing. 2D floor plan to WebGPU 3D walkthrough with a live material estimate and GST-ready quotation; 300+ unit tests and 136 pgTAP database assertions. TypeScript, Fastify, Supabase, Kotlin. |
| **[small-model-agents](https://github.com/salimkt/small-model-agents)** | Reference implementation of reliable agents on small models: schema-validated tool calling, tiered routing, evidence-based escalation, an MCP server, and an eval harness whose CI gate blocks regressions. Python stdlib. |
| **[web-share](https://github.com/salimkt/web-share)** · [live demo](https://salimkt.github.io/web-share/) | Peer-to-peer WebRTC file sharing as a PWA, with end-to-end-encrypted MQTT signalling or offline QR pairing. No server, no accounts. |

<p>
  <a href="https://salimkt.github.io/DataRat/"><img src="https://github.com/salimkt/DataRat/raw/main/docs/overview.png" alt="DataRat executive dashboard with KPI cards, a Holt-Winters forecast and generated key findings" width="49%"></a>
  <a href="https://salimkt.github.io/3xdezine/"><img src="https://github.com/salimkt/3xdezine/raw/main/docs/screenshots/studio.jpg" alt="3xDezine studio with floor plan editor, WebGPU 3D view and live estimate" width="49%"></a>
</p>

### Stack

`Python` `FastAPI` `Django` `Celery` `vLLM` `Ollama` `Hugging Face` `PyTorch` `LangChain` `CrewAI` `MCP`
`Cassandra` `pgvector` `Qdrant` `FAISS` `PostgreSQL` `DuckDB` `Redis` `Kafka` `RabbitMQ`
`Whisper` `NVIDIA Canary` `Tacotron2` `LayoutLMv3` `PaddleOCR-VL` `Qwen-VL`
`Kubernetes` `Docker` `GCP` `GitLab CI` `GitHub Actions`
`TypeScript` `React` `React Native` `three.js` `Kotlin`

---

AI/ML engineer at Netstratum Technologies since June 2022. Open to roles in the UAE/Gulf, Europe (with relocation) and remote: **mohdsalimkt@gmail.com**
