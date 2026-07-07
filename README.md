# LIVO AI: Pronunciation Evaluator 🎙️

LIVO AI is a full-stack, AI-powered application designed to evaluate speech pronunciation with granular phonetic accuracy. By comparing spoken audio against a reference script, the system highlights exact mispronunciations, skipped sounds, and extra syllables, all while maintaining strict **Zero-Retention Data Privacy**.

## ✨ Key Features
* **Granular Phonetic Feedback:** Breaks down words into individual sounds (phonemes) and color-codes accuracy.
* **Local ML Pipeline:** Uses OpenAI's Whisper (tiny) for robust Automatic Speech Recognition (ASR) without relying on expensive third-party APIs.
* **G2P Translation:** Converts both the expected script and the spoken transcript into CMUdict Arpabet phonemes for mathematical comparison.
* **DPDP Act 2023 Compliant:** Engineered with a "Zero Retention" protocol. Audio is processed purely in volatile RAM/Temp files and immediately destroyed after inference. No databases, no logs.
* **Modern UI:** Built with Next.js and Tailwind CSS for a sleek, responsive, and intuitive user experience.

---

## 🏗️ System Architecture

The project utilizes a decoupled architecture, connected via a single GitHub Meta-Repo:

* **Frontend (`/front`):** Next.js / React (Hosted on Vercel)
* **Backend (`/back`):** FastAPI / Python (Hosted on Hugging Face Spaces Docker Container)

> **Note:** This repository uses Git Submodules to link the frontend and backend codebases.

---
