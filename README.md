# Retrieval-Augmented Generation (RAG) Example Project

This repository demonstrates a simple, educational implementation of Retrieval-Augmented Generation (RAG) in Python. RAG is a powerful technique that combines information retrieval with generative models, allowing LLMs to answer questions using both their internal knowledge and external data sources.

## 🚀 Project Motivation

Traditional language models are limited to the data they were trained on. RAG enables dynamic, up-to-date, and context-aware responses by retrieving relevant information from external datasets or knowledge bases at inference time.

This project is a minimal, hackable starting point for anyone interested in:
- Building their own RAG pipelines
- Experimenting with embeddings and vector search
- Understanding the basics of retrieval-augmented LLMs

## ✨ Features

- Loads a dataset of cat facts from a text file
- (Optional) Embeds text chunks using a local or remote embedding model
- Stores embeddings in an in-memory vector database (list)
- Ready to extend with retrieval and generation logic
- Simple, readable Python code

## 📁 Directory Structure

```
rag_from_scratch/
├── cat-facts.txt         # Sample dataset (cat facts)
├── rag_from_scratch.py   # Main script: loads data, prepares for RAG
├── README.md             # Project documentation
```

## ⚡️ Quickstart

### 1. Clone the Repository

```sh
git clone https://github.com/singh-krishan/rag_from_scratch.git
cd rag_from_scratch
```

### 2. (Optional) Create a Virtual Environment

```sh
python3 -m venv .venv
source .venv/bin/activate
```

### 3. Install Dependencies

If you plan to use embedding models or additional features, install dependencies:
```sh
pip install -r requirements.txt
```
*(If requirements.txt is not present, install as needed for your extensions.)*

### 4. Run the Script

```sh
python rag_from_scratch.py
```

## 📝 Example Output

```
Loaded 100 entries
Added chunk 1/100 to the database
Added chunk 2/100 to the database
...
```

## 🛠️ How to Extend

- **Add Retrieval:** Implement a function to search for the most relevant cat fact(s) given a user query.
- **Integrate LLM:** Use a language model (e.g., via Ollama, Hugging Face, or OpenAI) to generate answers using retrieved facts.
- **Swap Dataset:** Replace `cat-facts.txt` with your own knowledge base or documents.
- **Persist Vector DB:** Use a real vector database (e.g., Chroma, FAISS, Pinecone) for scalable retrieval.

## 📚 References & Further Reading

- [Retrieval-Augmented Generation (RAG) Paper](https://arxiv.org/abs/2005.11401)
- [Hugging Face RAG Documentation](https://huggingface.co/docs/transformers/model_doc/rag)
- [Ollama Documentation](https://ollama.com/)
- [Chroma Vector DB](https://www.trychroma.com/)
- [OpenAI Cookbook: Retrieval-Augmented Generation](https://cookbook.openai.com/examples/retrieval_augmented_generation)

---

## 🤝 Contributing

Pull requests and suggestions are welcome! If you use this as a starting point for your own RAG experiments, let me know or open an issue.

---

Happy hacking! 🐱✨ 