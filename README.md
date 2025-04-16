# Multimodal-RAG-with-Weaviate-Google-Gemini

This project demonstrates a complete **Multimodal Retrieval-Augmented Generation (MM-RAG)** pipeline using **Weaviate** for vector-based image search and **Google Gemini 1.5 Flash** for vision-language generation.

Users can input natural language queries like `"fishing with my son"` or `"paragliding through the mountains"` and receive:
1. A semantically matched image.
2. A detailed, AI-generated description using Google's multimodal LLM.

---

## 🔁 Workflow Overview

- **Step 1:** Vector-based image retrieval with Weaviate (filtered by media type)
- **Step 2:** Image understanding & generation via Google Gemini 1.5 Flash
- **Step 3:** Result display using Markdown + inline visualization

---

## 🧰 Tools & Technologies

| Category         | Tools Used                            |
|------------------|----------------------------------------|
| Language         | Python                                 |
| Vector Database  | [Weaviate](https://weaviate.io/)       |
| Multimodal AI    | [Google Gemini 1.5 Flash](https://ai.google.dev/) |
| Libraries        | `weaviate-client`, `google-generativeai`, `Pillow`, `IPython`, `dotenv` |
| Deployment Ready | `.env` file for API key management     |

---

## 💡 Example Usage

```python
# Run a multimodal query
mm_rag("paragliding through the mountains")
