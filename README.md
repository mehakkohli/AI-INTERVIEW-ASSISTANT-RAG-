# 🤖 AI Interview Assistant (RAG-Based)

An intelligent **AI-powered interview preparation platform** that simulates real interview scenarios using your resume.
It combines **Retrieval-Augmented Generation (RAG)**, **LLMs**, and **voice interaction** to deliver a personalized interview experience.

---

## 🚀 Features

✨ **Resume-Based Question Generation**

* Upload your resume (PDF)
* AI generates role-specific interview questions based on your profile

🧠 **RAG-Powered Intelligence**

* Uses vector search (FAISS) + embeddings
* Ensures questions are grounded in your resume

🎤 **Voice + Text Interaction**

* Answer using text or voice
* Speech-to-text and text-to-speech enabled

📊 **Answer Evaluation**

* AI evaluates your answers
* Provides feedback + score

📄 **Final Performance Report**

* Strengths
* Weaknesses
* Improvement plan

---

## 🧩 Tech Stack

* **Frontend:** Streamlit
* **Backend:** Python
* **LLM:** Groq (LLaMA 3.1)
* **Embeddings:** Sentence Transformers (`all-MiniLM-L6-v2`)
* **Vector DB:** FAISS
* **Speech:** Whisper + TTS
* **RAG Pipeline:** Custom implementation

---

## 🏗️ Project Structure
├── app.py                # Main Streamlit app
├── interview_engine.py   # RAG-based question generation
├── rag_engine.py         # Chunking + embeddings + retrieval
├── rag_pipeline.py       # Knowledge-based Q&A (optional RAG)
├── resume_parser.py      # Extract text from PDF
├── resume_analyzer.py    # Resume insights
├── evaluation.py         # Answer evaluation
├── voice_module.py       # Voice recording + STT + TTS
├── data/
│   └── interview_qa.txt  # Knowledge base
├── .env                  # API keys

## 🧠 How RAG Works in This Project

1. Resume is split into chunks
2. Chunks are converted into embeddings
3. Stored in FAISS vector database
4. Relevant chunks are retrieved based on role
5. LLM generates questions using retrieved context

👉 This ensures:

* No generic questions
* Fully personalized interview

---

## 🎯 Usage Flow

1. Upload your resume
2. Analyze resume (optional)
3. Select job role
4. Start interview
5. Answer via text or voice
6. Get feedback + final report

---

## 📸 Example Output

* “Can you explain your experience with machine learning models in your project?”
* “How did you optimize performance in your application?”

👉 Questions are tailored to your resume

---

## ⚠️ Notes

* First run may take time (model download)
* Voice feature works best with microphone enabled
* Whisper runs on CPU (may be slightly slow)

---

## 💡 Future Improvements

* Add real-time feedback during answers
* Improve scoring accuracy
* Add more domain-specific question banks
* Deploy on cloud (Streamlit Cloud / AWS)

---

## 🙌 Acknowledgements

* Sentence Transformers
* FAISS
* Groq API
* Open-source AI community

---

## 📌 Author

**Vinay Sharma**
AI & Data Enthusiast

---
