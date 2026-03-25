# Multimodal MCTS Summarizer

A multimodal text summarization system powered by Monte Carlo Tree Search (MCTS). Supports text, image, and video inputs with five specialised agents. 

## Features
- 🧠 **MCTS Optimization**: Selects the best summary from five agents using UCT search.
- 🖼️ **Multimodal Input**: Process text, images, and video files.
- 🤖 **Five Summarization Agents**:
  - Extractive – extracts key facts verbatim.
  - Abstractive – rewrites concisely in own words.
  - Bullet Points – presents key points.
  - TLDR – ultra‑concise summary.
  - Detailed – comprehensive, longer summary.

## Quick Start

### 1. Clone the repository
git clone https://github.com/Sakshi-Dodke/Summarizer-Agent.git
cd Summarizer-Agent

### 2. Set up Python environment
python -m venv venv
venv\Scripts\activate      # Windows
pip install -r requirements.txt

If requirements.txt is missing, install manually:
pip install flask requests opencv-python Pillow werkzeug nltk pandas

### 3. Pull Required Ollama Models
ollama pull llama3.2:latest
ollama pull llava:7b

### 4. Start Backend Server
python app.py
