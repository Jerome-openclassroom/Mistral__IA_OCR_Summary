<img src="https://upload.wikimedia.org/wikipedia/en/c/c3/Flag_of_France.svg" width="100px" height="auto" />

# Résumé météo OCR automatisé — Projet démonstratif IA 🇫🇷

![EUstack](https://img.shields.io/badge/🇪🇺%20EUstack-ready-blue)
![SouverainAI](https://img.shields.io/badge/🇫🇷%20SouverainAI-oui-success)
![OCR_Ready](https://img.shields.io/badge/📷%20OCR--ready-Mistral-blue)
![LLM_Mistral](https://img.shields.io/badge/🧠%20LLM-Mistral_Small-lightblue)
![Realtime](https://img.shields.io/badge/⚡%20Realtime--processing-yes-brightgreen)



Ce dépôt présente un projet complet de démonstration d’un pipeline IA 100% fonctionnel, permettant de transformer une image de notes météo manuscrites en un **résumé lisible, structuré et envoyé automatiquement par email**, le tout en utilisant :

- ✅ **Mistral OCR** (modèle français de reconnaissance optique)
- ✅ **Mistral Small (LLM)** pour la synthèse automatique
- ✅ **n8n** pour l’orchestration no-code du flux
- ✅ **Google Sheet** pour l’archivage automatique

## Objectif
Montrer qu’un **document manuscrit réel**, même en italique ou stylisé, peut être :
- lu correctement sans fine-tuning OCR,
- synthétisé automatiquement en langage naturel,
- envoyé et archivé en autonomie via un workflow moderne.

---

## 🗂️ Arborescence du dépôt

- `README.md` : version française
- `README_En.md` : version anglaise / english version

### 📁 `code/`
- `n8n_Mistral_blueprint.json` : blueprint exporté du workflow n8n pour reproduction
- `n8n_Mistral_Notebook.ipynb` : notebook Python pour encoder l’image et déclencher le webhook n8n

### 📁 `screenshots/`
- `Easy_Test.png` : image test initiale, produite depuis un document MS Word avec texte météo fictif en italique
- `mail_easy_test.png` : mail reçu après traitement de `Easy_Test.png`
- `Real_Test.png` : scan de véritables notes météo personnelles (été 2017)
- `mail_real_test.png` : mail reçu après traitement de `Real_Test.png`
- `saved_summary.png` : aperçu de la ligne archivée dans Google Sheet (texte + date)
- `Workflow.png` : capture du workflow n8n en mode graphique

---

## 🚀 Résultat

- La reconnaissance OCR, même sur une **police italique manuscrite**, est **excellente** grâce à Mistral.
- Le résumé généré est **fluide, cohérent et professionnel**, y compris sur des documents réels.
- Le tout est **automatisé** (upload → OCR → LLM → mail + sauvegarde) sans besoin d'intervention humaine.

⏱️ **Temps de traitement total** : quelques secondes par image, y compris la synthèse.

---

## 🔁 Reproductibilité

Ce projet est **100% reproductible** :
- via n8n avec l’import du blueprint fourni,
- ou via le script Python pour tester le webhook en local ou depuis Colab.

---

## 🙌 Technologies utilisées 🇪🇺

- [n8n.io](https://n8n.io) 🇩🇪
- [Mistral AI](https://mistral.ai/fr) 🇫🇷 
- Google Sheets (via n8n) 🇺🇸

---

📄 Rapport technique généré par Mistral (“Le Chat”)

Dans ce document PDF, Le Chat met en lumière les capacités de notre dépôt à travers l’intégration de Mistral Mini et Mistral OCR. Une synthèse illustrée, produite en réponse au prompt :

_"Regardes, Le Chat : Tu es à l'honneur sur mon dernier dépôt GitHub, consacré à Mistral IA !"_

👉 [Consulter le rapport](./)

---

## 📅 Date de génération du présent README

11/08/2025

