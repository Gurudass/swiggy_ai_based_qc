<h1 align="center">🚀 Swiggy AI-Based Quality Control (QC) Engine</h1>

<p align="center">
  <b>Automated Enterprise Call Analytics, Disposition & QA with Generative AI</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python" />
  <img src="https://img.shields.io/badge/FastAPI-Framework-teal?style=for-the-badge&logo=fastapi" />
  <img src="https://img.shields.io/badge/OpenAI_%2F_LLM-Integrated-purple?style=for-the-badge&logo=openai" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" />
</p>

---

## 📌 Overview
An enterprise-grade automated Quality Control (QC) pipeline engineered to evaluate 50K–100K daily customer interaction records. Designed to reduce manual QA overhead by 70–80%, extracting structured insights, customer sentiments, intent analysis, and objection tracking with sub-second processing throughput.

## ✨ Key Features
- **Automated Disposition & Sentiment Tagging:** Leverages structured LLM prompts for multi-class classification and sentiment profiling.
- **RAG & Guardrail Verification:** Assesses policy compliance and minimizes hallucination on customer credit card offers.
- **Real-Time Analytics Dashboard:** Aggregates intent distributions, objection trends, and agent performance metrics.
- **Multi-channel Triggering:** Integrated with Meta WhatsApp Cloud API for automated post-call customer communications.

## 🛠️ Architecture & Tech Stack
- **Backend:** Python, FastAPI, WebSockets
- **AI/ML:** Whisper (Speech-to-Text), LLM Inference (vLLM / Sarvam-M / OpenAI), Silero VAD
- **Storage:** MySQL / SQLite, Redis Caching
- **DevOps:** Docker, AWS EC2 / S3

## ⚡ Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/Gurudass/swiggy_ai_based_qc.git
cd swiggy_ai_based_qc
```

### 2. Set up virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: .\venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Environment Variables
Create a `.env` file in the root folder:
```env
OPENAI_API_KEY=your_key_here
DATABASE_URL=sqlite:///./qc_database.db
PORT=8000
```

### 4. Run the API
```bash
uvicorn main:app --reload --port 8000
```
Interactive API documentation will be available at `http://localhost:8000/docs`.

---

## 👨‍💻 Author
**Guru Das**  
Senior Full-Stack & GenAI Engineer  
- GitHub: [@Gurudass](https://github.com/Gurudass)  
- LinkedIn: [Guru Das](https://linkedin.com)
