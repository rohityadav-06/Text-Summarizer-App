# 📝 Text Summarizer App (FastAPI + T5)

## 🚀 Project Overview

This project is a **Text Summarization Web App** built using: - FastAPI
(Backend) - Hugging Face Transformers (T5 Model) - PyTorch - Jinja2
(Frontend)

It takes a dialogue/text input and generates a concise summary using a
fine-tuned T5 model.

------------------------------------------------------------------------

## ✨ Features

-   🔹 Text Summarization using T5
-   🔹 FastAPI REST API
-   🔹 Simple Web UI (HTML)
-   🔹 GPU / CPU Support
-   🔹 Clean text preprocessing

------------------------------------------------------------------------

## 📂 Project Structure

    ├── app.py                # Main FastAPI app
    ├── saved_summary_model/  # Trained T5 model
    ├── index.html            # Frontend UI

------------------------------------------------------------------------

## ⚙️ Installation

### 1. Clone Repository

``` bash
git clone <your-repo-link>
cd your-project-folder
```

### 2. Install Dependencies

``` bash
pip install fastapi uvicorn transformers torch jinja2
```

------------------------------------------------------------------------

## ▶️ Run the App

``` bash
uvicorn app:app --reload
```

Open in browser:

    http://127.0.0.1:8000

------------------------------------------------------------------------

## 🔌 API Endpoint

### POST /summarize/

**Request Body:**

``` json
{
  "dialogue": "Your input text here"
}
```

**Response:**

``` json
{
  "summary": "Generated summary"
}
```

------------------------------------------------------------------------

## 🧠 How It Works

1.  Input text is cleaned using regex
2.  Tokenized using T5 tokenizer
3.  Model generates summary using beam search
4.  Output is decoded into readable text

------------------------------------------------------------------------

## 📌 Requirements

-   Python 3.8+
-   PyTorch
-   Transformers

------------------------------------------------------------------------

## 👨‍💻 Author

Rohit Yadav

------------------------------------------------------------------------

## ⭐ Future Improvements

-   Add file upload (PDF/Text)
-   Add multi-language support
-   Improve UI design
-   Deploy on cloud (AWS/Render)
