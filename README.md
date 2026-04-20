# ⚡ LLM Performance Observability Dashboard

A real-time benchmarking dashboard for comparing LLM models across key performance metrics — built by **Sagar Chaudhary**, Performance Engineering Lead @ PwC India.

![Dashboard Preview](preview.png)

## 🎯 What It Does

Benchmarks and visualizes performance of 5 LLM models:
- **GPT-4o** & **GPT-4o-mini** (OpenAI)
- **Claude 3 Haiku** & **Claude 3 Sonnet** (Anthropic)
- **Gemini 1.5 Flash** (Google)

## 📊 Metrics Tracked

| Metric | Description |
|--------|-------------|
| **TTFT** | Time to First Token (ms) |
| **P50/P95/P99 Latency** | Response time percentiles |
| **Token Throughput** | Output tokens per second |
| **Cost per 1K Tokens** | Cost efficiency analysis |
| **Success Rate** | Error rate under load |
| **Concurrency Impact** | Latency vs concurrent users |

## 🏗️ Real-World Context

This dashboard is inspired by actual work done at **PwC India** benchmarking 5 LLM models for an Insurance chatbot:
- Reduced P99 latency from **7s → 1.8s** (74% reduction)
- Achieved **71% token cost reduction** via prompt compression
- Recommended **Claude 3 Haiku** as production model based on lowest TTFT (0.7s)

## 🚀 Run Locally

```bash
git clone https://github.com/sagar9804644867/llm-performance-dashboard
cd llm-performance-dashboard
pip install -r requirements.txt
streamlit run app.py
```

## 🔌 Connect Your Own Data

Replace the simulated data in `app.py` with real data from:
- **LangSmith** exports (JSON/CSV)
- **JMeter JTL** files
- **Datadog** metric exports
- **Custom API logs**

## 🛠️ Tech Stack

- **Streamlit** — Dashboard UI
- **Plotly** — Interactive charts
- **Pandas** — Data processing
- **NumPy** — Statistical calculations

## 📬 Contact

**Sagar Chaudhary** — Performance Engineering Lead  
🌐 [Portfolio](https://sagar-portfolio-new.vercel.app)  
💼 [LinkedIn](https://linkedin.com/in/sagar-chaudhary-024254130)  
📧 sagar98chaudhary19@gmail.com
