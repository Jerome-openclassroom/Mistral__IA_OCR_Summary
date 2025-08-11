<img src="https://upload.wikimedia.org/wikipedia/en/c/c3/Flag_of_France.svg" width="100px" height="auto" />

# Automated Weather Report from OCR — 🇫🇷 Mistral-Powered Demo Project

This repository showcases a complete AI-powered pipeline, turning a handwritten weather log image into a **clean, structured summary automatically emailed and archived**, using:

- ✅ **Mistral OCR** (French high-performance optical character recognition)
- ✅ **Mistral Small (LLM)** for natural language synthesis
- ✅ **n8n** for orchestration and automation
- ✅ **Google Sheets** for archiving

## Objective

Demonstrate that a **real handwritten document**, even in stylized italic fonts, can be:
- accurately read without OCR fine-tuning,
- summarized in fluent, professional French,
- sent and archived automatically via a modern no-code workflow.

---

## 🗂️ Repository structure

- `README_En.md` : this English version
- `README.md` : French version

### 📁 `code/`
- `n8n_Mistral_blueprint.json`: exportable blueprint of the n8n workflow
- `n8n_Mistral_Notebook.ipynb`: Python notebook to encode an image and trigger the webhook

### 📁 `screenshots/`
- `Easy_Test.png`: synthetic image created in MS Word with fictional italic weather text
- `mail_easy_test.png`: email received after processing `Easy_Test.png`
- `Real_Test.png`: scanned weather logs from real handwritten notes (summer 2017)
- `mail_real_test.png`: email received after processing `Real_Test.png`
- `saved_summary.png`: example of the saved row in Google Sheets (summary + timestamp)
- `Workflow.png`: full view of the n8n workflow

---

## 🚀 Results

- OCR recognition, even on **stylized italic fonts**, was **outstanding** thanks to Mistral OCR.
- The generated summary was **fluent, accurate, and human-readable**, even for real documents.
- Everything is **fully automated** (upload → OCR → LLM → email + archive) with zero manual intervention.

⏱️ **End-to-end processing time**: a few seconds per image (including summarization).

---

## 🔁 Reproducibility

This project is **fully reproducible**:
- via n8n using the included workflow blueprint,
- or via the Python notebook to send test images.

---

## 🙌 Technologies used

- [n8n.io](https://n8n.io)
- [Mistral AI](https://mistral.ai/fr)
- Google Sheets (via n8n integrations)

---

## 📅 README generation date

August 11, 2025
