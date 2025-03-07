# Chat with Your Data: RAG-Enhanced LLM Conversations

A **Retrieval-Augmented Generation (RAG)** pipeline for interacting with the book *"Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow"* by Aurélien Géron. This project allows you to **ask questions** and get **accurate, context-aware answers** directly from the book's content using advanced natural language processing techniques.

---

## 🚀 Features

- **Interactive Q&A**: Ask questions about machine learning concepts, algorithms, and techniques covered in the book.
- **RAG Pipeline**: Combines retrieval (FAISS + embeddings) and generation (LLM) for accurate and context-aware answers.
- **Preprocessing**: Extracts, cleans, and chunks the book's text for efficient retrieval.
- **Scalable**: Easily extendable to other books or datasets.
- **Open-Source**: Built using free and open-source tools like Hugging Face Transformers, Sentence Transformers, and FAISS.

---

## 🛠️ Technologies Used

- **Embeddings**: `all-MiniLM-L6-v2` (Sentence Transformers)
- **Generative Model**: `Qwen/Qwen2.5-1.5B-Instruct` (Hugging Face Transformers)
- **Vector Database**: FAISS (Facebook AI Similarity Search)
- **Text Extraction**: PyMuPDF (fitz)
- **Programming Language**: Python

---

## 📖 How It Works

1. **Text Extraction**: The book's text is extracted from the PDF and preprocessed into smaller chunks.
2. **Embeddings**: Each chunk is converted into a vector using a pre-trained embedding model (`all-MiniLM-L6-v2`).
3. **FAISS Index**: The embeddings are indexed using FAISS for fast similarity search.
4. **Retrieval**: When a question is asked, the system retrieves the most relevant chunks from the book.
5. **Generation**: A generative model (`Qwen/Qwen2.5-1.5B-Instruct`) generates an answer based on the retrieved context.

---

## 💻 Getting Started

### Prerequisites

- Python 3.7+
- Install required libraries:
  ```bash
  pip install faiss-cpu pymupdf sentence-transformers transformers

## 🌟 Example Questions

- "What is the difference between supervised and unsupervised learning?"
- "How does gradient descent work?"
- "What is the purpose of a validation set?"
- "Explain the cost function of KNN."

---

## 🚧 Future Enhancements

- Add support for other books or datasets.
- Fine-tune the generative model on the book's content for better performance.
- Deploy the pipeline as a web app or chatbot.

---

## 🤝 Contributing

Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request.

---

## 🙏 Acknowledgments

- Aurélien Géron for the amazing book *"Hands-On Machine Learning with Scikit-Learn, Keras, and TensorFlow"*.
- Hugging Face for the `transformers` library and pre-trained models.
- Facebook AI Research for FAISS.

---

Enjoy chatting with your data! 🚀
