# 🎥 AI-Powered YouTube Video & Meeting Analysis Assistant

An AI-powered application that analyzes YouTube videos and meeting recordings using a Retrieval-Augmented Generation (RAG) pipeline.

The system automatically transcribes audio, generates concise summaries, extracts key insights, identifies action items and decisions, and allows users to ask questions about the content through a conversational AI interface.

---

# 🚀 Features

## 🎙️ Audio & Video Processing
- Upload meeting recordings
- Analyze YouTube videos
- Automatic audio extraction
- Speech-to-text transcription using Whisper

## 📝 AI Summarization
- Executive summary generation
- Detailed meeting notes
- Topic-wise breakdown
- AI-generated titles

## ✅ Action Item Extraction
- Tasks discussed in meetings
- Assigned responsibilities
- Deadlines and commitments
- Follow-up actions

## 🎯 Key Decision Detection
- Important decisions made
- Conclusions reached
- Agreement points

## 🔍 RAG-Based Question Answering
- Chat with meeting content
- Ask contextual questions
- Retrieve relevant transcript chunks
- Generate accurate AI responses

## 💾 Vector Database Storage
- Embedding generation
- Semantic search
- Context retrieval using ChromaDB

---

# 🏗️ Project Architecture

```text
User
 │
 ▼
Streamlit Frontend
 │
 ▼
Audio / Video Input
 │
 ▼
Whisper Transcription
 │
 ▼
Transcript Generation
 │
 ├── Summary Generator
 │
 ├── Action Item Extractor
 │
 ├── Decision Extractor
 │
 ▼
Embedding Creation
 │
 ▼
ChromaDB Vector Store
 │
 ▼
LangChain RAG Pipeline
 │
 ▼
Mistral / Gemini LLM
 │
 ▼
Question Answering
```

---

# 📂 Directory Structure

```text
AI-Meeting-Analyzer/
│
├── app.py
│
├── frontend/
│   └── streamlit_ui.py
│
├── Core/
│   ├── transcriber.py
│   ├── summarizer.py
│   ├── extractor.py
│   └── rag_engine.py
│
├── utils/
│   └── audio_processor.py
│
├── downloads/
│
├── .env
├── .env.example
├── requirements.txt
└── README.md
```

---

# 🛠️ Tech Stack

## Frontend
- Streamlit

## AI & NLP
- OpenAI Whisper
- LangChain
- Mistral AI / Gemini AI

## Vector Database
- ChromaDB

## Embeddings
- Sentence Transformers

## Backend
- Python

## Environment Management
- dotenv

---

# ⚙️ Installation

## Clone Repository

```bash
git clone https://github.com/yourusername/AI-Meeting-Analyzer.git

cd AI-Meeting-Analyzer
```

## Create Virtual Environment

```bash
python -m venv .venv
```

### Windows

```bash
.venv\Scripts\activate
```

### Linux / Mac

```bash
source .venv/bin/activate
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 🔑 Environment Variables

Create a `.env` file:

```env
GOOGLE_API_KEY=your_google_api_key
MISTRAL_API_KEY=your_mistral_api_key
```

---

# ▶️ Run Application

```bash
streamlit run app.py
```

Application will start on:

```text
http://localhost:8501
```

---

# 📋 Workflow

### Step 1
Upload a meeting recording or provide a YouTube URL.

### Step 2
System extracts audio.

### Step 3
Whisper transcribes speech into text.

### Step 4
Transcript is processed for:

- Summary generation
- Action item extraction
- Decision extraction

### Step 5
Transcript chunks are converted into embeddings.

### Step 6
Embeddings are stored in ChromaDB.

### Step 7
LangChain retrieves relevant chunks.

### Step 8
LLM generates contextual answers.

---

# 💡 Example Questions

```text
What was discussed about project deadlines?

Who is responsible for deployment?

What decisions were finalized?

Summarize the entire meeting.

What are the pending action items?
```

---

# 📊 Use Cases

- Business Meetings
- Team Standups
- Project Discussions
- Client Calls
- Educational Lectures
- YouTube Learning Videos
- Research Interviews

---

# 🔮 Future Improvements

- Speaker Identification
- Multi-language Support
- FastAPI Backend
- Real-Time Meeting Analysis
- PDF Report Export
- Email Summary Generation
- Meeting Calendar Integration

---

# 🎯 Learning Outcomes

This project demonstrates:

- Generative AI
- Retrieval-Augmented Generation (RAG)
- Vector Databases
- LangChain Framework
- Speech Recognition
- LLM Integration
- Semantic Search
- End-to-End AI Application Development

---

# 👨‍💻 Author

Ankush Patial

AI Video & Meeting Insight Assistant using RAG Pipeline

Built using Python, Streamlit, Whisper, LangChain, ChromaDB, and Mistral/Gemini AI.
