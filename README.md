# Hi there, I'm Dylan 👋

## 🎯 About Me
I am an AI developer passionate about building reliable autonomous agents and local-first systems. My focus is on moving beyond simple prototypes to learn the engineering realities of **production-grade AI**—including distributed systems, local inference, and multi-agent orchestration.

My portfolio is designed to demonstrate these skills through end-to-end applications that solve real-world problems using modern, privacy-focused stacks.

* **LinkedIn:** [https://www.linkedin.com/in/datadrivendylan/](https://www.linkedin.com/in/datadrivendylan/)
* **Email:** dylangamachefl@gmail.com

---

## 🛠️ Core Competencies & Skills

My skills are organized by the core domains required for building robust AI systems.

| Domain | Technologies & Concepts |
| :--- | :--- |
| **🤖 Agentic AI & RAG** | **Ollama** (Local LLMs), Langchain, Hybrid Search (BM25 + Vector), **Qdrant**, **FAISS**, Structured Output (Pydantic/Zod) |
| **🏗️ Backend & Systems** | **Redis Streams** (Event Bus), **FastAPI**, Docker Compose, Microservices, Async/Await, GPU Optimization (CUDA) |
| **💻 Web & Edge AI** | **WebLLM** (Browser-based WASM), **React 19**, TypeScript, Web Workers, **SQLite WASM**, Next.js, Tailwind CSS |
| **🛡️ Reliability & Ops** | PII Redaction (Microsoft Presidio), Distributed Locking, LLM Evaluation (RAGAs), DSPy, GitHub Actions |
| **📈 Data & Analytics** | Pandas, NumPy, Scikit-learn, XGBoost, LightGBM, SQL, Plotly |

---

## 🚀 AI Projects

This is a showcase of my hobby projects, each built to explore specific engineering challenges like distributed processing, client-side inference, and computer vision.

### 1. Project: PodScribe - Distributed Transcription & RAG
A production-grade monorepo for automated podcast processing, summarization, and chat. It coordinates multiple AI services using an event-driven architecture.

* **Repo:** [GitHub](https://github.com/dylangamachefl/pod-scribe)

**Key Features:**
* **`Distributed Systems`:** Uses **Redis Streams** to decouple the transcription worker, summarization service, and RAG engine, ensuring reliable message processing and scalability.
* **`Hardware Optimization`:** Implements a custom **Distributed GPU Lock** with an "Immediate Release" strategy to efficiently share CUDA resources between WhisperX (transcription) and Ollama (inference).
* **`Hybrid Search`:** Combines keyword search (BM25) with vector similarity (Qdrant) using **Reciprocal Rank Fusion (RRF)** for high-accuracy retrieval.

### 2. Project: Fantasy Football Chatbot V2 (Edge AI)
A sophisticated, **100% client-side** conversational agent. Unlike traditional chatbots, this runs the LLM entirely in the user's browser for zero-latency, private analysis.

* **Repo:** [GitHub](https://github.com/dylangamachefl/fantasy-football-chatbot-v2)

**Key Features:**
* **`Browser-Based Inference`:** Utilizes **WebLLM** and **WASM** to run multi-billion parameter models (Qwen) directly on the client, removing the need for a backend API.
* **`Teacher-Student Loop`:** Implements a "flywheel" where a larger local model (Ollama) acts as a "Teacher" to generate synthetic data and optimize prompts for the smaller browser-based "Student" model.
* **`Dynamic Context`:** Uses smart semantic routing to prune complex SQL schemas, fitting them into the limited context window of browser-based models.

### 3. Project: Grocery Deal Finder (Multi-Agent Vision)
An intelligent system that uses computer vision and a map-reduce pipeline to extract and match deals from weekly grocery ads against a user's shopping list.

* **Repo:** [GitHub](https://github.com/dylangamachefl/grocery-deal-finder)

**Key Features:**
* **`Multi-Agent Orchestration`:** A 4-agent pipeline (Vision Extractor, Librarian, Interpreter, Matcher) powered by **Google Gemma 3** to handle distinct stages of data processing.
* **`Map-Reduce`:** Implements parallel processing to handle large inventories, splitting items into shards for concurrent analysis by the "Inventory Librarian" agent.
* **`Client-Side Vectors`:** Runs **Transformers.js** in a Web Worker to classify thousands of products using vector embeddings locally, keeping the UI responsive.

### 4. Project: DocuQuery - Local-First Privacy RAG
A professional-grade RAG assistant designed for 100% data privacy. All parsing, embedding, and inference happen locally on the user's hardware to prevent data leakage.

* **Repo:** [GitHub](https://github.com/dylangamachefl/docuquery)

**Key Features:**
* **`Privacy-First Architecture`:** Ensures 100% local processing by orchestrating **Ollama** and **FAISS** (in-memory vector store) via Docker, keeping data off external clouds.
* **`Security Guardrails`:** Integrates **Microsoft Presidio** to automatically detect and redact PII (Names, Emails, SSNs) from user inputs before they reach the LLM.
* **`Evaluation Pipeline`:** Includes a dedicated container running **RAGas** to quantitatively measure retrieval "Faithfulness" and "Context Precision".

---

## 📊 Foundational Projects & Business Acumen

A collection of projects that demonstrate my foundational ML skills, full-stack capabilities, and ability to connect technical solutions to business impact.

* **Project: End-to-End Data Science for Business Impact**
    * **Description:** A portfolio of three end-to-end data science projects demonstrating strong business acumen. These projects (Customer Churn, Demand Forecasting, and Credit Risk) show my ability to connect complex ML models (XGBoost, LightGBM) to direct financial outcomes (e.g., +1,100% ROI, $2.1M in projected savings).
    * **Repo:** [GitHub Repo](https://github.com/dylangamachefl/data-analytics-portfolio)

* **Project: WTStats - Full-Stack Application**
    * **Description:** A comprehensive, high-performance web application built with **Next.js, React, TypeScript, and Tailwind CSS**. Demonstrates skills in full-stack development and **Static Site Generation (SSG)** for a reliable, production-ready user experience.
    * **Repo:** [GitHub - wtstats-nextjs](https://github.com/dylangamachefl/WTStats)

* **Project: Hugging Face Mini-App Collection**
    * **Description:** A monorepo of smaller web apps built to demonstrate proficiency with the Hugging Face ecosystem (Transformers, Inference API, and Spaces), covering foundational NLP and Computer Vision tasks.
    * **Repo:** [GitHub - huggingface-project-suite](https://github.com/dylangamachefl/huggingface-project-suite)

---
