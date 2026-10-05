<h1 align="center">Muhammed Salim K T</h1>

<p align="center">
  <strong>AI/ML Engineer — LLM systems, RAG, agent orchestration, speech &amp; vision</strong><br>
  4+ years shipping production AI · Kochi, India · open to remote worldwide
</p>

<p align="center">
  <a href="mailto:mohdsalimkt@gmail.com">mohdsalimkt@gmail.com</a> ·
  <a href="https://linkedin.com/in/muhammed-salim-k-t">LinkedIn</a>
</p>

---

I build production LLM systems end to end — agent orchestration, retrieval, model serving, and the evaluation that keeps them honest.

### What I have built

**A multi-agent / tool-calling engine.** I authored `bm-agent-engine`, the orchestration layer behind an on-premise enterprise LLM platform, as a drop-in replacement for its CrewAI-based stack — roughly 49,000 lines of Python. A 73-toolset registry, ReAct agents with tiered escalation, structured delegate/ask/finish delegation, and a FAST/SMALL/LARGE/THINKING router over vLLM and Ollama. Re-architecting it so the model makes only narrow, schema-validated decisions let a **12B model do the work the previous stack needed a 32B model for** — enough GPU saving to run the whole platform on a single node. It cut over with one config change, because the SSE event contract was preserved exactly.

**RAG at 10M+ embeddings.** Chunking, Sentence-Transformers embeddings, a Cassandra vector-store schema tuned for similarity search, and hybrid BM25 + dense retrieval with re-ranking. Served behind vLLM at **1.8s median latency and 99.7% uptime**, and +45% answer accuracy over the bare LLM baseline.

**Speech, both directions.** Whisper STT at 94% accuracy and Tacotron2 TTS, with live captioning shipped into a production video-calling product at 92%.

**Vision and documents.** PaddleOCR-VL and Qwen-VL served through Transformers with CUDA and attention-implementation tuning; four OCR engines wired into the retrieval pipeline; LayoutLMv3 fine-tuned to **91% F1** across 100K+ documents a month.

**The platform under it.** Kubernetes across eight environments including two GPU/DGX clusters — Kustomize overlays, StatefulSets, PDBs, RBAC, cert-manager TLS.

### Side project: 3xDezine

**[3xDezine](https://github.com/salimkt/3xdezine)** · [live demo](https://salimkt.github.io/3xdezine/) · [Android APK](https://github.com/salimkt/3xdezine/releases/download/android-latest/3xdezine.apk)

A house and interior design tool: draw a floor plan in 2D, walk it in 3D, apply real building materials, and get a live material estimate. Rendering is three.js on **WebGPU** with image-based lighting, AgX tone mapping, GTAO, screen-space GI and reflections, and a sun that follows its real path over Mumbai. Costing is in rupees with per-material wastage, whole-pack rounding and a contingency buffer, priced from the **Maharashtra PWD Schedule of Rates**. Plan edits are checked live against **NBC 2016** room minimums, and when a change breaks one the engine proposes the nearest edit that doesn't. Includes a review mode with cost deltas, 8 Indian plan templates, and a native Android client (Jetpack Compose + Filament). First paint is **86 KB** gzipped; the 3D engine loads while you pick a template.

### Stack

`Python` `FastAPI` `vLLM` `Ollama` `Hugging Face` `PyTorch` `LangChain` `CrewAI`
`Qdrant` `FAISS` `pgvector` `Pinecone` `Cassandra` `Redis` `Kafka`
`Whisper` `Tacotron2` `LayoutLMv3` `PaddleOCR` `OpenCV`
`Kubernetes` `Docker` `GCP` `GitLab CI` `React` `React Native` `TypeScript`
`three.js` `WebGPU` `Kotlin` `Jetpack Compose` `Fastify` `PostgreSQL`

---

Currently an AI/ML engineer at Netstratum Technologies. Open to remote roles worldwide — **mohdsalimkt@gmail.com**.
