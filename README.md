# Telugu Story Generator Using a Tiny Decoder-Only Transformer

A web-based Generative AI application that generates Telugu stories based on user-provided topics and story categories using a custom-built Tiny Decoder-Only Transformer.

## 📌 Project Overview

The **Telugu Story Generator** is a Generative AI project designed to generate Telugu stories from short user prompts.

The application uses a custom decoder-only Transformer architecture implemented using PyTorch. Users can enter a topic, select a story category, and generate Telugu text through an interactive web interface.

The project combines frontend development, backend API integration, and deep learning to explore language generation for Telugu.

## 🎯 Objectives

- Generate Telugu stories from user-provided topics.
- Implement a Tiny Decoder-Only Transformer from scratch.
- Explore next-token prediction using causal self-attention.
- Develop an interactive web application.
- Improve Telugu text generation through better datasets and tokenization.
- Explore Retrieval-Augmented Generation (RAG) for contextual story generation.

## 🛠️ Technology Stack

| Component | Technology |
|---|---|
| Frontend | React.js, Vite, HTML, CSS |
| Backend | Python, FastAPI, Uvicorn |
| AI/ML | PyTorch |
| Model Architecture | Decoder-Only Transformer |
| Tokenization | Word-Level Telugu Tokenizer |
| Database | MongoDB Atlas |
| Vector Database | Chroma (planned) |
| Programming Languages | Python, JavaScript |
| Development Tools | VS Code, Git, GitHub |

## 🏗️ System Architecture

The application follows a frontend-backend-model architecture.

1. **User Interface:** Users enter a topic and select a story category through the React interface.
2. **API Request:** The frontend sends the request to the FastAPI backend.
3. **Tokenization:** The Telugu tokenizer converts the input text into numerical token IDs.
4. **Transformer Model:** The PyTorch decoder-only Transformer predicts the next tokens using causal self-attention.
5. **Text Generation:** The generated token sequence is converted back into Telugu text.
6. **Output Display:** The generated story is displayed on the web interface.

## 🧠 Model Architecture

The project implements a Tiny Decoder-Only Transformer consisting of:

- Token Embeddings
- Positional Embeddings
- Causal Self-Attention
- Output Layer
- Next-Token Prediction

The model generates text autoregressively, predicting one token at a time based on previously generated tokens.

## ✨ Key Features

- Telugu story generation.
- Topic-based text generation.
- Story category selection.
- Custom Transformer architecture.
- Interactive React-based interface.
- FastAPI backend integration.
- Experimental AI-powered text generation.



## ⚙️ Installation and Setup

### Prerequisites

- Python
- Node.js and npm
- Git
- Visual Studio Code

### 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd Telugu-Story-Generator
```

### 2. Backend Setup

Navigate to the backend directory:

```bash
cd backend
```

Create a virtual environment:

```bash
python3 -m venv venv
```

Activate the environment:

**macOS / Linux**
```bash
source venv/bin/activate
```

**Windows**
```bash
venv\Scripts\activate
```

Install the required dependencies:

```bash
pip install torch fastapi uvicorn numpy pymongo python-dotenv
```

Start the FastAPI server:

```bash
uvicorn main:app --reload
```

### 3. Frontend Setup

Open another terminal and navigate to the frontend directory:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Open the local URL displayed in the terminal to access the application.

*Note: The commands assume the conventional folder structure and entry points shown above.*

## 🗄️ Database Integration

MongoDB Atlas is being integrated to store:

- User story requests.
- Generated story outputs.
- Related metadata.

Chroma vector database is planned for implementing Retrieval-Augmented Generation (RAG).

## 🚀 Future Enhancements

- Expand and clean the Telugu story dataset.
- Improve the Telugu tokenizer and vocabulary.
- Enhance story fluency and contextual relevance.
- Integrate MongoDB for persistent storage.
- Implement RAG using Chroma vector database.
- Compare prompting, retrieval, and fine-tuning approaches.
- Evaluate generation quality, repetition, latency, and cost.

## 📊 Project Evaluation

The system aims to be evaluated using the following parameters:

- **Relevance:** How closely the generated story matches the user's topic.
- **Fluency:** Readability and grammatical quality of Telugu text.
- **Repetition:** Frequency of repeated words and phrases.
- **Latency:** Time taken to generate a story.
- **Cost:** Computational resources required for generation.

## ⚠️ Current Limitations

The current prototype is trained on a small sample collection of Telugu stories. Therefore, generated outputs are experimental and may contain:

- Repeated words or sentences.
- Incomplete sentences.
- Limited vocabulary.
- Reduced contextual consistency.

These limitations will be addressed through dataset expansion, improved tokenization, and model experimentation.

## 👨‍💻 Project Team

| Name | Student ID |
|---|---|
| V Sameer Reddy | 2520030276 |
| V Gautam | 2520030316 |
| S. Ashwanth Reddy | 2520030081 |

**Project Guide:** Dr. V. Anu Ragavi  
**Department:** Computer Science and Engineering  
**Institution:** KL University  
**Academic Year:** 2026–2027

---

## 📜 License

This project is developed for academic purposes as part of the Generative AI and AI Platform Engineering course.
