# 🇪🇸 HablaAI – AI-Powered Spanish Language Learning Assistant

**HablaAI** is an ongoing NLP-based project aimed at helping Spanish learners improve their grammar and language proficiency through automated linguistic analysis and personalised feedback.

The project focuses on analysing Spanish sentences, identifying grammatical inconsistencies, and providing meaningful explanations to support language learning.

> 🚧 **Project Status: In Development**

## 🎯 Objectives

- Analyse Spanish sentences using Natural Language Processing.
- Identify grammatical errors and linguistic inconsistencies.
- Provide contextual grammar explanations and correction suggestions.
- Support European Spanish (es-ES) conventions.
- Build a foundation for personalised and adaptive Spanish learning.

## 🛠️ Tech Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Backend Framework | FastAPI |
| NLP Library | spaCy |
| Language Model | es_core_news_sm |
| API Server | Uvicorn |

## ✨ Implemented Features

- **Linguistic Analysis:** Tokenisation, lemmatisation, Part-of-Speech tagging and morphological analysis.
- **Initial Grammar Detection:** Prototype for identifying potential past-tense inconsistencies using temporal markers.
- **Modular Architecture:** Separate grammar-analysis modules for different linguistic concepts.
- **REST API:** FastAPI-based backend for exposing language analysis functionality.

## 🏗️ Project Structure

```text
HablaAI/
│
├── backend/
│   ├── data/
│   ├── services/
│   │   └── grammar/
│   │       ├── __init__.py
│   │       ├── agreement.py
│   │       ├── analyzer.py
│   │       ├── pronouns.py
│   │       ├── ser_estar.py
│   │       └── verbs.py
│   │
│   ├── __init__.py
│   ├── grammar.py
│   └── main.py
│
├── .gitignore
└── README.md
```

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/HablaAI.git
cd HablaAI
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

### 3. Activate the environment

**Windows:**

```bash
.venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install fastapi uvicorn spacy
```

### 5. Download the Spanish NLP model

```bash
python -m spacy download es_core_news_sm
```

### 6. Run the backend

```bash
cd backend
uvicorn main:app --reload
```

Access the API documentation:

```text
http://127.0.0.1:8000/docs
```

## 🗺️ Development Roadmap

- [x] FastAPI backend setup
- [x] spaCy Spanish NLP integration
- [x] Basic linguistic analysis
- [x] Initial past-tense error detection
- [ ] Advanced verb conjugation analysis
- [ ] Subject–verb agreement detection
- [ ] Ser vs. Estar analysis
- [ ] Pronoun usage analysis
- [ ] Context-aware grammar correction
- [ ] Personalised learning feedback
- [ ] Frontend integration
- [ ] Speech recognition and conversational practice

## 🌍 Language Focus

HablaAI initially focuses on **European Spanish (es-ES)**, with consideration for regional grammatical conventions and vocabulary.

## 🤝 Future Scope

The long-term vision is to evolve HablaAI into an intelligent Spanish-learning companion that combines NLP, grammar analysis, conversational practice and personalised learning experiences.

---

**Developed by:** Goteti Sri Sai Varun

*Building HablaAI, one feature at a time.*
