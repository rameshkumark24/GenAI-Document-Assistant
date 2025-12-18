# 📄 GenAI Document Assistant

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Framework](https://img.shields.io/badge/Framework-Streamlit-red)
![AI](https://img.shields.io/badge/AI-Generative%20AI-green)

## 📌 Overview
**GenAI Document Assistant** is an intelligent AI-powered tool designed to help users interact with and extract insights from their documents. By leveraging Generative AI (LLMs) and Retrieval-Augmented Generation (RAG), this application allows users to upload documents (PDFs, TXT, DOCX) and ask natural language questions to get accurate, context-aware answers.

## 🚀 Key Features
* **📂 Multi-Format Support:** Upload and process PDFs, Text files, and Word documents.
* **💬 Interactive Chat:** Chat with your documents using a conversational interface.
* **🧠 Context-Aware Answers:** Uses advanced embeddings to retrieve specific sections of the document for accurate responses.
* **⚡ Fast Processing:** Efficient document chunking and vector search for real-time performance.

## 🛠️ Tech Stack
* **Programming Language:** Python
* **Frontend:** Streamlit
* **AI/LLM Orchestration:** LangChain / LlamaIndex (Assumed)
* **Vector Database:** FAISS / ChromaDB (Assumed)
* **Model Provider:** OpenAI GPT / Google Gemini / HuggingFace

## 📂 Project Structure
```text
genai-document-assistant/
│
├── src/
│   ├── app/
│   │   ├── main.py            # Main application entry point
│   │   └── utils.py           # Helper functions for processing
│   └── processing/
│       └── document_loader.py # Logic for reading files
│
├── data/                      # Folder for storing uploaded/processed files
├── requirements.txt           # Python dependencies
└── README.md                  # Project documentation

```

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone [https://github.com/rameshkumark24/genai-document-assistant.git](https://github.com/rameshkumark24/genai-document-assistant.git)
cd genai-document-assistant

```

### 2. Create a Virtual Environment

```bash
python -m venv venv
# Windows
.\venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

```

### 3. Install Dependencies

```bash
pip install -r requirements.txt

```

### 4. Set Up Environment Variables

Create a `.env` file in the root directory and add your API keys:

```env
OPENAI_API_KEY=your_openai_api_key_here
# or
GOOGLE_API_KEY=your_google_api_key_here

```

## ▶️ Usage

Run the application using Streamlit:

```bash
streamlit run src/app/main.py

```

The app will open in your browser at `http://localhost:8501`.

## 📸 Workflow

1. **Upload:** User uploads a document via the sidebar.
2. **Process:** The app splits the text into chunks and creates vector embeddings.
3. **Ask:** User types a question in the chat box.
4. **Retrieve & Answer:** The AI finds the relevant text chunks and generates an answer.

## 🤝 Contributing

Contributions are welcome! Please fork the repo and create a pull request.

## 📄 License

This project is licensed under the MIT License.
