# 🎥 AI Video Analysis Assistant

An AI-powered application that analyzes YouTube videos and allows users to interact with video content through intelligent question answering, summarization, and Retrieval-Augmented Generation (RAG).

---

## Features

### 🎬 YouTube Video Processing
- Extract audio from YouTube videos
- Support for public YouTube links

### 🎤 Speech-to-Text
- Automatic transcription of video content
- Converts audio into searchable text

### 📝 AI Summarization
- Generates concise summaries
- Highlights key insights from videos

### 🔍 Retrieval-Augmented Generation (RAG)
- Creates embeddings from transcripts
- Stores embeddings in ChromaDB
- Retrieves relevant context before answering

### 💬 AI Question Answering
- Ask questions about video content
- Context-aware responses using RAG pipeline

### 📚 Vector Database
- ChromaDB for semantic search
- Efficient retrieval of relevant transcript chunks

---

## Project Structure

```text
VIDEO AGENT
│
├── Core
│   ├── extractor.py
│   ├── transcriber.py
│   ├── summarizer.py
│   ├── rag_engine.py
│   └── vector_store.py
│
├── utils
│   └── audio_processor.py
│
├── downloades
│
├── vector_db
│
├── app.py
├── main.py
├── requirements.txt
└── README.md
```

## Tech Stack

### Frontend
- Streamlit

### Backend
- Python

### AI & NLP
- LangChain
- Google Gemini API
- Sentence Transformers

### Vector Database
- ChromaDB

### Video Processing
- yt-dlp
- FFmpeg
- pydub

---

## Installation

### Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/youtube-ai-video-assistant.git

cd youtube-ai-video-assistant
```

### Create Virtual Environment

```bash
python -m venv .venv
```

Activate Environment

Windows

```bash
.venv\Scripts\activate
```

Mac/Linux

```bash
source .venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Configure Environment Variables

Create `.env`

```env
GOOGLE_API_KEY=your_api_key
```

### Run Application

```bash
streamlit run app.py
```

---

## Future Scope

- Multi-language support
- Real-time video analysis
- PDF report generation
- Speaker identification
- Advanced sentiment analysis
- Cloud deployment support

---

## Author

Pratibha

AI Video Analysis Assistant Project
