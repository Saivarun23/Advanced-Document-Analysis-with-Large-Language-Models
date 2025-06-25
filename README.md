# Advanced-Document-Analysis-with-Large-Language-Models

A lightweight NLP pipeline for analyzing and understanding long PDF documents using Large Language Models (LLMs). This project focuses on extracting text from PDFs, summarizing content, and automatically generating relevant questions — all with minimal code and powerful transformer models.

---

## 🔍 Features

- 📥 **Text Extraction** from PDF using `pdfplumber`
- ✨ **Summarization** using `t5-small` from Hugging Face Transformers
- 🧩 **Passage Splitting** using NLTK's sentence tokenizer
- ❓ **Question Generation** using `valhalla/t5-base-qg-hl` model
- 💡 Sample analysis on Google’s Terms of Service (May 2024 version)

---

## 🛠️ Technologies Used

- Python 3.x
- [pdfplumber](https://github.com/jsvine/pdfplumber) for PDF parsing
- [Hugging Face Transformers](https://huggingface.co/transformers/)
  - `t5-small` for summarization
  - `valhalla/t5-base-qg-hl` for question generation
- [NLTK](https://www.nltk.org/) for sentence tokenization

---

## 📌 How It Works

1. **Extract PDF text** with `pdfplumber`
2. **Summarize** the beginning of the document using `t5-small`
3. **Split** full document into 200-word passages using NLTK
4. **Generate questions** from each passage using a question-generation model
5. **Print** passages alongside generated questions for document understanding

---

## 📁 Folder Structure

```
project/
├── Advanced_Document_Analysis_with_LLMs.ipynb   # Main notebook
├── example_pdfs/
│   └── google_terms_of_service_en_in.pdf
├── extracted_text.txt                           # Extracted raw text
└── README.md
```

---

## 🧠 Example Output

```text
Passage 1:
GOOGLE TERMS OF SERVICE...
Generated Questions:
- What does the Google Terms of Service cover?
- What are the Terms of Service?

Passage 2:
Besides these terms, we also publish a Privacy Policy...
Generated Questions:
- What is the name of the company that provides Google services?
```

---

## 🚀 Future Improvements

- Integrate semantic search using sentence embeddings
- Enhance summarization with larger models (e.g., `bart-large-cnn`)
- Add Named Entity Recognition (NER) for deeper legal understanding
- Package into a web app using Streamlit (optional for future)

---

## 📜 License

This project is for educational and portfolio purposes only. Make sure to respect copyright and fair use when analyzing proprietary documents.

---

## 🙌 Acknowledgments

- Hugging Face for their amazing NLP models
- NLTK and pdfplumber for the supporting tools

---
