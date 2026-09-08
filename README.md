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

### Stack

`Python` `FastAPI` `vLLM` `Ollama` `Hugging Face` `PyTorch` `LangChain` `CrewAI`
`Qdrant` `FAISS` `pgvector` `Pinecone` `Cassandra` `Redis` `Kafka`
`Whisper` `Tacotron2` `LayoutLMv3` `PaddleOCR` `OpenCV`
`Kubernetes` `Docker` `GCP` `GitLab CI` `React` `React Native` `TypeScript`

---

Currently an AI/ML engineer at Netstratum Technologies. Open to remote roles worldwide — **mohdsalimkt@gmail.com**.
