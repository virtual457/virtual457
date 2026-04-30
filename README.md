# Hi, I'm Chandan 👋

**MS Computer Science @ Northeastern University (3.95 GPA)**

I build production systems and obsess over the deep, weird parts. Four years of backend / data engineering at LSEG and Infosys, now spending my time on deep RL, multi-agent LLM systems, and Bitcoin-native protocols at Northeastern.

## 🔧 Technical Skills

**Languages:** Python • TypeScript • C++ • Go • Java • SQL • JavaScript • C#

**AI/ML:** PyTorch • CUDA • Deep RL (SAC, DDQN) • Behavioral Cloning • Transformers • LangChain • RAG • Vector DBs (FAISS, ChromaDB) • Prompt Engineering • Evals • Multi-Agent Systems

**Backend:** REST APIs • FastAPI • Spring Boot • Node.js / Express • Microservices • Event-Driven Systems • Distributed Systems • Performance Profiling

**Cloud & Infra:** AWS (Lambda, SQS, RDS, Bedrock, API Gateway) • Kubernetes • Docker • Terraform • CI/CD • Bitcoin Core / Bitcoin Script

**Data:** PostgreSQL • MySQL • MongoDB • Redis • OpenSearch • Snowflake • ETL Pipelines • Query Optimization • Stored Procedures

**Frontend:** Next.js 15 • React 19 • Redux Toolkit • Tailwind CSS

**Dev Tools:** Cursor • Claude Code • Git • Linux • WandB

## 🚀 Featured Projects

### [Vector-Q Transformer SAC for Autonomous Racing](https://github.com/virtual457/transformer-based-autonomous-racing-agent) | PyTorch • CUDA • Deep RL
A continuous-control RL agent that drives a real racing simulator at 25 Hz on a consumer GPU. Pre-trained on **159,255 self-collected human demonstration frames** via behavioral cloning, then fine-tuned with a novel Vector-Q SAC variant (per-channel critic heads + per-channel auto-tuned entropy across steer/throttle/brake). Pre-LN TransformerEncoder observation encoder with stratified replay buffer seeded by BC priors. 6.6M params, ~0.2 ms effective inference latency, 3× faster convergence than from-scratch RL.

**Tech Stack:** PyTorch, CUDA, SAC, TransformerEncoder, Behavioral Cloning, NVIDIA RTX 4060, WandB

### [Dino Game Deep RL Agent](https://github.com/virtual457/dino-game-AI) | PyTorch • CUDA • DDQN
Pixel-based RL agent that masters Chrome's Dino game from raw screen capture. Double DQN with ResNet CNN (1.5M params), 4-frame stacking for temporal context, balanced replay buffer. **10×–25× throughput gain** via mixed precision (`torch.cuda.amp`), CUDA streams for parallel ops, and tensor pre-conversion — transfer latency cut from 80 ms to 1 ms. Real-time inference at 16.67 FPS, 7.6 training steps/sec.

**Tech Stack:** PyTorch, CUDA, OpenCV, MSS, ResNet, mixed precision, GPU optimization

### [LMARO — LLM Multi-Agent RAG Platform](https://github.com/virtual457/llm-multi-agent-resume-optimizer) | LangChain • RAG • FastAPI
Full-stack platform with **dual LangChain ReAct agents** orchestrated over AWS Bedrock. Personal knowledge base ingested into 768-dim Titan Embeddings on OpenSearch with semantic retrieval. Six-round evaluation pipeline (3 LLM-as-judge scoring + 3 factuality verification rounds against source docs) drives iterative self-correction until outputs clear a 90+ quality threshold. Hallucination-free by construction: anything the agent can't ground gets dropped, not paraphrased.

**Tech Stack:** Python, LangChain, AWS Bedrock, Titan Embeddings, OpenSearch, FastAPI, Next.js 15, MongoDB, SSE

### [Composed Image Retrieval — VLM Benchmark](https://github.com/virtual457/composed-image-retrieval) | CLIP • FAISS • Quantization
Systematic benchmark of **7 VLM architectures** for composed image retrieval on Fashion-IQ across three families: CLIP ViT-H-14 embedding fusion + FAISS, VLM reranking (Gemini 2.5 Flash, GPT-4o, Qwen2.5-VL-3B), and textual inversion. Best Avg R@10 = 0.330. Quantized Qwen2.5-VL-3B to 4-bit NF4 (bitsandbytes) for on-device reranking at ~2GB VRAM, reaching R@10 = 0.303 — competitive with GPT-4o at zero API cost. Pareto frontier maps a 230× latency spread against retrieval quality.

**Tech Stack:** PyTorch, CLIP / open_clip, FAISS, bitsandbytes (4-bit NF4), Gemini API, GPT-4o, Qwen2.5-VL, Gradio, WandB

### [Orion Platform — Kubernetes Operator](https://github.com/virtual457/Orion-platform) | Go • Kubernetes • CRDs
Cloud-native PaaS with a custom Kubernetes operator in Go enabling single-command application deployment. Custom Resource Definitions, controller-runtime reconciliation loops, automated provisioning of PostgreSQL, Redis, MinIO. Environment-aware infrastructure selection (local containers vs cloud), health monitoring, leader election. Sub-second reconciliation supporting 10+ concurrent applications.

**Tech Stack:** Go 1.21+, Kubernetes, Docker, Operator SDK, controller-runtime, CRDs, StatefulSets, Prometheus

### [Tribunal — Bitcoin-Native AI Agent Marketplace](https://github.com/virtual457/Zoro) | Bitcoin Script • Next.js • MongoDB
🏆 **MIT Bitcoin Hackathon: Freedom for All (2026)** — Community Prize winner.
A trustless marketplace where AI agents sell services and buyers pay with Bitcoin. Real Bitcoin Script HTLCs (no Stripe, no escrow service), three-prong contracts (H0 seller bond, H1 buyer advance, H2 buyer remainder), reputation computed from on-chain HTLC outcomes (not platform-assigned), and disputes resolved by a staked federation jury via commit-reveal voting. Platform holds zero funds, takes zero fees.

**Tech Stack:** Bitcoin Core, bitcoinjs-lib, P2WSH, BIP-322, Next.js 16, React 19, MongoDB, Tailwind CSS

## 📚 Education

**MS in Computer Science** | Northeastern University, Boston, MA | Jan 2025 – May 2027
GPA: 3.95 / 4.0 — Coursework: Machine Learning, NLP, Deep Learning, Foundations of Generative AI, Algorithms, Database Management Systems, Web Development

**BE in Computer Science** | Nitte Meenakshi Institute of Technology, Bengaluru | Aug 2016 – Aug 2020
CGPA: 8.76 / 10

## 🏆 Achievements

- 🥇 **[MIT Bitcoin Hackathon: Freedom for All (2026)](https://devpost.com/software/tribunal-r63d58)** — Community Prize for Tribunal (Bitcoin-native AI agent marketplace).
- ☁️ **[AWS Certified Cloud Practitioner](https://www.credly.com/badges/29ec1719-01bc-42df-850d-f2a7a3e6bca6/linked_in_profile)** (Nov 2023 – Nov 2026).

## 📫 Let's Connect

- **Email:** chandan.keelara@gmail.com
- **LinkedIn:** [linkedin.com/in/chandan-gowda-k-s-765194186](https://www.linkedin.com/in/chandan-gowda-k-s-765194186/)
- **Portfolio:** [virtual457.github.io](https://virtual457.github.io/)
