Pixel 👓✨

Pixel is a high-performance, RAG-driven conversational partner designed to bridge the gap between a technical assistant and a personal companion. Unlike standard chatbots, Pixel uses persistent vector memory to ensure she never forgets a conversation or a shared project.
🧠 Core Features

    Persistent Long-Term Memory: Powered by ChromaDB, Pixel stores every interaction, allowing her to reference past conversations and "learn" your preferences over time.

    Knowledge Base Integration: Syncs local .txt and .md files into a searchable vector space using Recursive Character Splitting.

    Local-First & Private: Runs entirely on your machine using Ollama. No data leaves your IdeaPad.

    Personality-Driven: Built-in persona management that moves away from robotic "AI assistant" tropes toward a quirky, human-like partner.

🛠️ Tech Stack

    Language: Python 3.11+

    Brain: Ollama (dolphin-mistral, gemma2:2b, phi3:mini)

    Vector Database: ChromaDB

    Orchestration: LangChain (Text Splitters)

    Environment: UV / Virtualenv

🚀 Quick Start
1. Clone & Setup
Bash

git clone https://github.com/YOUR_USERNAME/pixel.git
cd pixel
python -m venv .venv
source .venv/bin/activate
pip install chromadb ollama langchain-text-splitters

2. Prepare the Brain

Make sure Ollama is running, then pull the recommended models:
Bash

ollama pull gemma2:2b
ollama pull phi3:mini

3. Run Pixel
Bash

python main.py

📂 Project Structure
Plaintext

pixel/
├── main.py           # The entry point & terminal interface
├── scripts/
│   ├── __init__.py    # Python package marker
│   ├── engine.py      # RAG logic & Persona management
│   └── utils.py       # SQLite fixes & performance tracking
├── knowledge/         # Drop your .txt files here to "teach" Pixel
└── chroma_db/         # Persistent vector storage (ignored by git)

🚧 Roadmap

    [x] v1.0 (Current): RAG implementation and Technical Partner persona.

    [ ] v2.0 (Next): Transition to "Companion Mode"—optimized for low-latency, emotional intelligence, and short-form banter.

    [ ] v2.1: Voice integration and image recognition.

📝 Author

Mohi (Mohd Talib) - Building digital brains on an IdeaPad.