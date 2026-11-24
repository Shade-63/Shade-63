# Dharmit Chauhan

**Building ML-powered security systems and low-latency Python backends.**  
Third-year Computer Science undergraduate at BMSIT&M, Bengaluru. I ship systems end-to-end, audit where they break, and harden them for production.

Open to remote **AI/ML Engineer**, **Python Backend (FastAPI/Flask)**, and **SDE** internships.

---

### Selected Work

**[Transformer-based WAF](https://github.com/Shade-63/transformer-waf) · [ONNX model](https://huggingface.co/Shade63/waf-onnx)** *(3-person team — ML & serving pipeline owned by me)*  
A Dockerized FastAPI reverse-proxy Web Application Firewall powered by a fine-tuned DistilBERT classifier running on ONNX Runtime. Engineered a 5-stage canonicalization normalizer (Unicode NFKC, double URL decoding, HTML entities, zero-width stripping, SQL hex escapes) and a 128-token sliding-window scanner (stride 64) to block padding-truncation evasions. Audited 15,791 captured HTTP requests to uncover header shortcut leakage and duplicate bias rather than relying on inflated in-distribution scores.  
`15.22 ms ONNX CPU latency · 1.57x p95 speedup · 84.09% OOD adversarial recall · 33/33 Pytest`

**[Sentinel-AI](https://github.com/Shade-63/Sentinel-AI) · [live demo](https://huggingface.co/spaces/Shade63/SentinelAI)**  
A multi-class scam and phishing detection service that goes beyond binary spam filtering to classify specific attack types—including financial fraud, romance scams, government impersonation, and bank phishing. Fine-tuned DistilBERT with hybrid rule-based post-processing, wrapped in a Dockerized Flask API with automated PDF incident reporting via ReportLab.  
`14,000-row dataset · 99.75% accuracy · 99.73% macro F1 · deployed on Hugging Face Spaces`

**FloodCast** *(tabular ML forecasting pipeline)*  
A multi-station hydrological forecasting pipeline built with LightGBM and Pandas across 5 river monitoring stations. Enforces leakage-free temporal train/test splits alongside leave-one-station-out (unseen-station) validation, tracking extreme-event tail error (`RMSE_top10`), `RMSE`, `MAE`, and `R²` to diagnose cross-basin distribution shift.  
`LightGBM · 5 river stations · temporal + unseen-station validation`

---

### Stack

```text
Languages     Python · Java · SQL · C · C++ (basics)
ML & NLP      Hugging Face Transformers · DistilBERT · ONNX Runtime · LightGBM · Scikit-learn · PyTorch · TensorFlow · Pandas · NumPy
Backend       FastAPI · Uvicorn · Pydantic v2 · Flask · SQLAlchemy · MySQL · SQLite · JWT
Infra & Test  Docker · Docker Compose · Pytest · Hugging Face Hub · Railway · Git
