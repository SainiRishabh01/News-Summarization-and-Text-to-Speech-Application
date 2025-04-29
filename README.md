# 📰 News Summarization & Text-to-Speech Application

## 🚀 Overview
This project is a **News Summarization and Text-to-Speech (TTS) Application** that fetches the latest news articles for a specific company, analyzes sentiment, and generates an audio summary in multiple languages. Built with **FastAPI** (backend) and **Streamlit** (frontend), it integrates web scraping, NLP, and text-to-speech technologies to offer an intuitive news analysis tool.

## 🔥 Features

- **🔍 News Scraping**: Fetches the latest news articles from **Bing News**.
- **📈 Sentiment Analysis**: Uses a pre-trained NLP model to analyze article sentiment.
- **📊 Comparative Analysis**: Displays sentiment distribution and topic overlap using visualizations.
- **🗣️ Text-to-Speech**: Converts summarized news into audio in **Hindi, English, Bengali, Spanish, and Tamil**.
- **✨ Interactive UI**: A user-friendly **Streamlit** interface for seamless interaction.
- **🎵 Audio Controls**: Play, Download, and Clear audio files.
- **🧠 Company Logo Fetching** using **Clearbit API**.
- **📊 Visualizations**: Pie & Bar charts for sentiment analysis using **Plotly**.
- **📄 JSON Output**: Structured JSON responses for summarized data & translations.

## 🛠️ Tech Stack

- **Python** 🐍 (Core programming language)
- **FastAPI** ⚡ (High-performance API framework)
- **Streamlit** 🖥️ (Frontend UI framework)
- **BeautifulSoup** 📰 (Web scraping library - No JavaScript required)
- **Transformers** 🤗 (Pre-trained NLP models for sentiment analysis)
- **gTTS** 🔊 (Google Text-to-Speech conversion)
- **Pandas** 📊 (Data manipulation & analysis)
- **NLTK** 📖 (Natural language processing)
- **Plotly** 📈 (Interactive charts)
- **Clearbit API** 🏢 (Company logo fetching)
- **googletrans** 🌍 (Translation using Google Translate API)
- **Selenium** 🕵️ (For advanced web scraping - Minimal usage)

## 🔧 Installation

### 1️⃣ Clone the repository
```bash
   git clone https://github.com/SainiRishabh01/News-Summarization-and-Text-to-Speech-Application.git
   cd News-Summarization-and-Text-to-Speech-Application
```

### 2️⃣ Set up a virtual environment (Recommended)
```bash
   conda create -p venv python==3.12
   source venv/bin/activate  
```

### 3️⃣ Install dependencies
```bash
   pip install -r requirements.txt
```

### 4️⃣ Run the FastAPI backend
```bash
   uvicorn api:app --reload
```

### 5️⃣ Run the Streamlit frontend
```bash
   streamlit run app.py
```

### 6️⃣ Access the application
- **FastAPI backend**: [http://127.0.0.1:8000](http://127.0.0.1:8000)
- **Streamlit frontend**: [http://localhost:8501](http://localhost:8501)

## 📌 Usage Guide

### ✅ Fetch News Articles
- Enter the company name (e.g., **"Google"**, **"Tesla"**).
- Click **"Fetch News"** to retrieve the latest articles.

### ✅ Analyze Sentiment & View Results
- The app displays sentiment analysis, summaries, and comparative analysis.
- Results are available in **JSON format** for further processing.

### ✅ Listen to Audio Summary
- The application generates an **audio summary** of the news in multiple languages.
- **Play or download** the audio summary directly.

### ✅ Clear Audio
- Click **"Clear Audio"** to remove generated files.

## 🌍 API Endpoints

🔹 **GET `/news/{company_name}`**  
- Fetches latest news articles and sentiment analysis.  
  Example: `http://127.0.0.1:8000/news/Google`

🔹 **GET `/tts/{text}`**  
- Converts provided text into speech (Hindi by default).  
  Example: `http://127.0.0.1:8000/tts/Hello%20World`

## 📂 Project Structure

```
├── api.py             # FastAPI backend
├── app.py             # Streamlit frontend
├── utils.py           # Web scraping, sentiment analysis, TTS, and processing
├── requirements.txt   # Python dependencies
```

## 🙌 Acknowledgments

- **Hugging Face** 🤗 for NLP models.
- **Google** 🔊 for gTTS.
- **Streamlit** 🎨 for easy UI development.

