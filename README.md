<h1 align="center">Sanchit Gupta</h1>
<h3 align="center">AI Infrastructure Engineer</h3>

<p align="center">
  <i>I keep large language models running on GPUs that have no internet connection.</i>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/sanchit-gupta-15a1b9229/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:sanchitguptaghj@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://1-sanchit-1.github.io/site/">
    <img src="https://img.shields.io/badge/Website-0B6B70?style=for-the-badge&logo=vitepress&logoColor=white" alt="Website" />
  </a>
  <img src="https://komarev.com/ghpvc/?username=1-Sanchit-1&label=Profile%20views&color=0b6b70&style=for-the-badge" alt="Profile views" />
</p>

---

### The system I work on

At **Neuralix.ai** I build and operate **EKAM AI**, an indigenous Defence AI-as-a-Service platform
launched under the MoD iDEX ADITI 2.0 initiative. It runs inside secure air-gapped sites, so every
package, model weight and upgrade has to be carried in offline.

```
                          ┌────────────────────────────────┐
      client  ───────────▶│   FastAPI gateway  ·  React    │
                          └────────────────┬───────────────┘
                                           │
                ┌──────────────────────────┼──────────────────────────┐
                ▼                          ▼                          ▼
       ┌─────────────────┐        ┌─────────────────┐        ┌─────────────────┐
       │  vLLM           │        │  NVIDIA Triton  │        │  Qdrant         │
       │  LLMs · SLMs    │        │  OCR · VLM      │        │  vector search  │
       │  cont. batching │        │  reranking      │        │  RAG retrieval  │
       └────────┬────────┘        └────────┬────────┘        └─────────────────┘
                └────────────┬─────────────┘
                             ▼
                    ┌─────────────────┐        ┌──────────────────────────┐
                    │   NVIDIA GPU    │◀──────▶│ Prometheus · Grafana     │
                    └─────────────────┘        └──────────────────────────┘

                  ── no egress · no package mirror · no second chances ──
```

---

### What I spend my time on

| | |
|---|---|
| **Serving** | Tuning continuous batching, KV-cache sizing and request scheduling so a fixed number of GPUs serves more users at lower latency. |
| **Model lifecycle** | Benchmarking open-source LLMs, VLMs, OCR, embedding and reranking models, then promoting them from evaluation into production. |
| **Air-gapped delivery** | Offline package mirrors, model-weight distribution, VDI deployments and standalone application packaging. |
| **Debugging** | Root-cause analysis that runs from a React bug all the way down to a CUDA driver fault. |

---

### Featured

**[AI-inference](https://github.com/1-Sanchit-1/AI-inference)** — a self-hosted, GPU-accelerated AI
platform on Kubernetes. An OpenAI-compatible endpoint served by vLLM, a FastAPI RAG service backed
by Qdrant, and a full observability stack (Prometheus, Grafana, Loki, Tempo, OpenTelemetry). Twenty
numbered, idempotent shell phases take a clean Ubuntu host to a working platform in one command.
Ships a CPU-only Docker Compose path too, so it runs on a laptop with no GPU.

---

### Stack

**Serving & GPU**

![vLLM](https://img.shields.io/badge/vLLM-1A1A2E?style=flat-square)
![NVIDIA Triton](https://img.shields.io/badge/NVIDIA%20Triton-76B900?style=flat-square&logo=nvidia&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-76B900?style=flat-square&logo=nvidia&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square)

**Backend**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)

**Platform**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![NGINX](https://img.shields.io/badge/NGINX-009639?style=flat-square&logo=nginx&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

**Observability & Frontend**

![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=flat-square&logo=opentelemetry&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

---

<p align="center">
  <img src="https://streak-stats.demolab.com?user=1-Sanchit-1&theme=transparent&hide_border=true&border_radius=4&date_format=M%20j%5B%2C%20Y%5D" alt="GitHub streak" />
</p>

<p align="center">
  <sub>B.Tech CSE, IIIT Lucknow '25 · LeetCode Knight (1891), 1000+ solved · Delhi, India</sub>
</p>
