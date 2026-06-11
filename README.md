# 🛡️ Intelligent Phishing & Scam Detection System

### Industrial Oriented Mini Project Project — MGIT, Department of Emerging Technologies
**Students:** D Sai Prakash (23261A6611) | Mekala VishnuVardhan (23261A6628)
**Guide:** Dr. Barnali Gupta Banik | Dr. Shaik Irfan Babu

---

## 📌 Project Overview
A multi-modal AI framework that detects phishing emails, malicious URLs,
and brand impersonation attacks in real time.

| Engine | Model | Target |
|--------|-------|--------|
| Linguistic | DistilBERT (fine-tuned) | Email text — Safe / Spam / Phishing |
| Lexical | Random Forest (18 features) | URL structure analysis |
| Visual | CLIP ViT-B/32 (zero-shot) | Brand logo verification |
| XAI | SHAP + LIME | Explainable evidence per prediction |

---

## 📊 Results

| Engine | F1 Score |
|--------|----------|
| Lexical (Random Forest) | 0.9629 |
| Linguistic (DistilBERT) | ~0.94 |
| Visual (CLIP) | ~0.90 |
| **Fused System** | **> 0.97** |

---

## 🚀 How to Run

1. Open `Phishing_Detection_Improved.ipynb` in **Google Colab**
2. Set runtime → **T4 GPU**
3. Run Cell 1 (Master Setup) first — mounts Google Drive
4. Run cells top to bottom in order
5. Models save automatically to Google Drive

> **Note:** DistilBERT training takes ~45–60 min on T4 GPU.
> After first run, models reload from Drive in ~2 min.

---

## 📁 Files in this Repository

| File | Description |
|------|-------------|
| `Training_Project_fixed(1).ipynb` | Complete Colab notebook — all 20 cells |
| `Email_threat)detection_fixed.ipynb` | Loading the models  |
| `email_threat_detection_doc.pdf` | Full project documentation |

> **Trained models (too large for GitHub) are shared via Google Drive:**
> [Click here to access models folder]https://drive.google.com/drive/folders/1DvoRrtggH3_E2wpANauYHoLq3hab0Wbq

---

## 🗂️ Dataset Sources

| Dataset | Source | Access |
|---------|--------|--------|
| Phishing emails | HuggingFace — ealvaradob/phishing-dataset | Free API |
| Spam/Ham emails | HuggingFace — SetFit/enron_spam | Free API |
| Malicious URLs | Kaggle — sid321axn/malicious-urls-dataset | Kaggle API |

---

## 🛠️ Tech Stack
Python 3.10 · PyTorch · HuggingFace Transformers · OpenAI CLIP
scikit-learn · SHAP · LIME · tldextract · FastAPI · Gradio · MLflow
Google Colab T4 GPU · Google Drive

---

## 🏛️ College Details

**Mahatma Gandhi Institute of Technology (Autonomous)**
Affiliated to JNTUH · Kokapet, Gandipet, Hyderabad - 500075
Department of Emerging Technologies · 2025–2026
