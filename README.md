# FAI_S3

# 🎓 Amrita UniBot: AI-Powered Campus Assistant

![Project Status](https://img.shields.io/badge/Status-Active-success)
![Python Version](https://img.shields.io/badge/Python-3.8%2B-blue)
![Framework](https://img.shields.io/badge/Streamlit-1.28.2-FF4B4B)
![AI Model](https://img.shields.io/badge/Model-GPT--4o--mini-orange)

**Amrita UniBot** is an intelligent, AI-driven conversational assistant designed specifically for **Amrita Vishwa Vidyapeetham, Coimbatore Campus**. It serves as a 24/7 support system for students, automating responses regarding academics, campus facilities, admissions, and student life.

Unlike standard rule-based chatbots, UniBot leverages **Large Language Models (LLMs)** and **Vector Search (RAG)** to provide context-aware, accurate, and personalized interactions.

---

##  Table of Contents
- [Key Features](#-key-features)
- [Technical Architecture](#️-technical-architecture)
- [Tech Stack](#️-tech-stack)
- [Installation & Setup](#-installation--setup)
- [Usage](#-usage)
- [Analytics & Metrics](#-analytics--metrics)
- [Future Scope](#-future-scope)
- [The Team](#-the-team)

---

##  Key Features

###  1. Secure Authentication System
* **Student Login:** Secure registration and login using student roll numbers.
* [cite_start]**Security:** SHA-256 hashing with salt for password protection[cite: 31, 231].
* **Session Management:** Persistent login sessions for user convenience.

###  2. AI-Powered Conversations
* [cite_start]**Intelligent Reasoning:** Integrated with **OpenRouter API** using the **GPT-4o-mini** model for natural, human-like dialogue[cite: 29].
* [cite_start]**Context Awareness:** Remembers previous turns in the conversation to maintain flow and context[cite: 232].

###  3. Advanced Memory & Knowledge Base
* [cite_start]**RAG Architecture:** Utilizes **ChromaDB** (Vector Database) to store and retrieve conversation history and institutional knowledge[cite: 30, 233].
* **Semantic Search:** Performs similarity-based context retrieval rather than simple keyword matching.
* [cite_start]**Verified Data:** Responses are grounded in a curated knowledge base of Amrita University facts (hostels, courses, rules)[cite: 147].

###  4. Feedback & Analytics
* [cite_start]**User Feedback:** Integrated 1-5 star rating system for response quality[cite: 234].
* [cite_start]**Dashboard:** Tracks metrics like session duration, message volume, and user satisfaction[cite: 258].

---

##  Technical Architecture

The system follows a modular architecture ensuring scalability and maintainability.

1.  **User Interface:** Streamlit frontend for chat and authentication.
2.  **Orchestrator:** Python backend manages session state and data flow.
3.  **Knowledge Retrieval:** ChromaDB vector store fetches relevant context.
4.  **Generation:** OpenRouter API (GPT-4o-mini) generates the final response.
5.  [cite_start]**Storage:** SQLite database stores User Profiles, Chat Logs, and Feedback[cite: 237].

**Data Flow:**
`User Input` ➡ `Auth Check` ➡ `Context Retrieval (ChromaDB)` ➡ `Prompt Engineering` ➡ `LLM (GPT-4o)` ➡ `Response`

---

## 🛠️ Tech Stack

| Component | Technology | Description |
| :--- | :--- | :--- |
| **Frontend** | Streamlit | Interactive web interface |
| **Language** | Python 3.11 | Core logic and scripting |
| **AI Model** | GPT-4o-mini | Via OpenRouter API |
| **Vector DB** | ChromaDB | Semantic memory and RAG |
| **Database** | SQLite | User data and structured logs |
| **Auth** | hashlib (SHA-256) | Security and hashing |
| **API** | REST/Requests | External model communication |

---

## 🚀 Installation & Setup

Follow these steps to set up the project locally.

### Prerequisites
* Python 3.8 or higher
* An API Key from [OpenRouter](https://openrouter.ai/)

rname/amrita-unibot.git](https://github.com/your-username/amrita-unibot.git)
cd amrita-unibot
