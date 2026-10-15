# Swiggy AI Quality Control (QC) Engine

**Enterprise Speech Analytics, Automated Dispositions, and LLM-Driven Quality Assurance**

---

### Overview
An automated quality-control and speech-analytics platform built to evaluate 50,000–100,000 daily customer interactions. Developed to replace manual QA overhead by 70–80%, extracting structured disposition insights, sentiment analysis, customer intent classification, and objection detection with sub-second latency.

---

### Key Capabilities

* **Automated Disposition & Intent Profiling:** Uses structured LLM prompt pipelines to classify multi-class customer dispositions and sentiment metrics.
* **RAG & Guardrail Compliance:** Ensures policy compliance and eliminates hallucinations on Swiggy credit card offer data via targeted context retrieval.
* **Operational Analytics:** Real-time metrics tracking objection types, campaign reach, and agent handover quality.
* **Automated Multi-Channel Follow-ups:** Event-driven integration with Meta WhatsApp Cloud API for instantaneous post-interaction confirmation.

---

### Architecture & Technical Stack

* **Backend Services:** Python, FastAPI, WebSockets, REST APIs
* **Speech & AI Engine:** Whisper (STT), Silero VAD, vLLM / Sarvam-M, OpenAI API
* **Data Storage & Caching:** MySQL, SQLite, Redis
* **Infrastructure:** Docker, AWS EC2, S3, Linux

---

### Getting Started

#### Prerequisites
* Python 3.10+
* Virtual environment tool (`venv` or `conda`)

#### 1. Clone the repository
```bash
git clone https://github.com/Gurudass/swiggy_ai_based_qc.git
cd swiggy_ai_based_qc
```

#### 2. Environment Setup
```bash
python -m venv venv
source venv/bin/activate  # Windows: .\venv\Scripts\activate
pip install -r requirements.txt
```

#### 3. Configuration
Create a `.env` file in the root directory:
```env
OPENAI_API_KEY=your_api_key
DATABASE_URL=sqlite:///./qc_engine.db
PORT=8000
```

#### 4. Launch the Application
```bash
uvicorn main:app --reload --port 8000
```
Interactive API documentation will be available at `http://localhost:8000/docs`.

---

### Author
**Guru Das**  
Senior Full-Stack & Generative AI Engineer  
[GitHub Profile](https://github.com/Gurudass)
