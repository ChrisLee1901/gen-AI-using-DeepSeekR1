# 🧠 Gen-AI-With-Deep-Seek-R1

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.0+-red.svg)](https://streamlit.io/)
[![LangChain](https://img.shields.io/badge/LangChain-0.1+-green.svg)](https://langchain.com/)

> **Intelligent AI Application integrating DeepSeek-R1 for Programming and Document Processing**

## 🌟 Overview

Gen-AI-With-Deep-Seek-R1 is a powerful AI application built on the Streamlit platform, integrating the DeepSeek-R1 model through Ollama. The project provides two main features:

- **🚀 DeepSeek Code Companion**: AI programming assistant with debugging and code consulting capabilities
- **📘 DocuMind AI**: RAG (Retrieval-Augmented Generation) system for analyzing and answering questions from PDF documents

## ✨ Key Features

### 🔧 DeepSeek Code Companion
- 🐍 **Python Expert**: Python specialist with deep and broad knowledge
- 🐞 **Debugging Assistant**: Support for code debugging and performance optimization
- 📝 **Code Documentation**: Automatic code documentation generation
- 💡 **Solution Design**: Solution design and architecture planning
- 🎨 **Dark Theme UI**: Beautiful dark interface, developer-friendly

### 📚 DocuMind AI
- 📄 **PDF Processing**: Process and analyze PDF documents
- 🔍 **Intelligent Search**: Smart information search within documents
- 💬 **Chat Interface**: Intuitive chat interface for asking questions
- 🧠 **RAG System**: RAG system with vector database for accurate answers

## 🚀 Installation and Setup

### System Requirements
- Python 3.8+
- Ollama with DeepSeek-R1 model
- 4GB RAM or more

### Step 1: Install Ollama and DeepSeek-R1

```bash
# Install Ollama
curl -fsSL https://ollama.ai/install.sh | sh

# Download DeepSeek-R1 models
ollama pull deepseek-r1:1.5b
ollama pull deepseek-r1:3b
```

### Step 2: Clone repository

```bash
git clone https://github.com/ChrisLee1901/Gen-AI-With-Deep-Seek-R1.git
cd Gen-AI-With-Deep-Seek-R1
```

### Step 3: Install dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Run the application

```bash
# Run Code Companion
streamlit run app.py

# Run DocuMind AI
streamlit run rag_deep.py
```

## 🎯 Usage

### DeepSeek Code Companion
1. Open browser and navigate to `http://localhost:8501`
2. Select appropriate DeepSeek-R1 model
3. Enter programming questions or paste code for debugging
4. Get detailed solutions with strategic print statements

### DocuMind AI
1. Run `streamlit run rag_deep.py`
2. Upload PDF file for analysis
3. Ask questions about document content
4. Get answers based on document context

## 🛠️ Technology Stack

| Technology | Description |
|-----------|-------------|
| **Streamlit** | Python web app framework |
| **LangChain** | AI application development framework |
| **Ollama** | Local AI model platform |
| **DeepSeek-R1** | Powerful AI reasoning model |
| **PDFPlumber** | PDF processing library |
| **Vector Database** | Embedding storage for RAG |

## 📁 Project Structure

```
Gen-AI-With-Deep-Seek-R1/
├── app.py                 # DeepSeek Code Companion
├── rag_deep.py           # DocuMind AI with RAG
├── requirements.txt      # Dependencies
├── LICENSE              # GPL v3 License
├── README.md           # Documentation
└── document_store/     # PDF storage directory (auto-created)
    └── pdfs/
```

## 🔧 Customization

### Change AI Model
```python
# In app.py or rag_deep.py
llm_engine = ChatOllama(
    model="deepseek-r1:7b",  # Change model
    base_url="http://localhost:11434",
    temperature=0.3  # Adjust creativity
)
```

### Customize Interface
Edit CSS in the `st.markdown()` section to change theme and colors.

## 🤝 Contributing

We welcome contributions from the community!

1. Fork the repository
2. Create a new branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Create a Pull Request

## 📝 Roadmap

- [ ] Support for additional document formats (Word, Excel, PowerPoint)
- [ ] Integration with other AI models
- [ ] Export functionality for results
- [ ] Multi-language support
- [ ] API endpoints for integration
- [ ] Docker deployment

## 🐛 Bug Reports

If you encounter any bugs, please create an issue on GitHub with:
- Detailed description of the bug
- Steps to reproduce
- Environment details (OS, Python version, etc.)
- Screenshots (if applicable)

## 📄 License

This project is released under the [GPL v3 License](LICENSE).

## 🙏 Acknowledgments

- [DeepSeek](https://www.deepseek.com/) for the powerful AI model
- [Ollama](https://ollama.ai/) for the local model platform
- [LangChain](https://langchain.com/) for the AI framework
- [Streamlit](https://streamlit.io/) for the web framework

---
