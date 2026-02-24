<div align="center">

# ⬡ VANTAGE
### Advanced Local Intelligence OS

*Private. Performant. Precise.*

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=flat-square&logo=python)
![Streamlit](https://img.shields.io/badge/Frontend-Streamlit-FF4B4B?style=flat-square&logo=streamlit)
![Ollama](https://img.shields.io/badge/Inference-Ollama-black?style=flat-square)
![ChromaDB](https://img.shields.io/badge/VectorDB-ChromaDB-orange?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

</div>

---

## What is VANTAGE?

VANTAGE is a high-performance, **local-first RAG (Retrieval-Augmented Generation)** platform built for secure, private document intelligence. Every model, every embedding, every vector — runs entirely on your hardware. No APIs. No telemetry. No compromise.

It's designed for analysts, researchers, and developers who need to extract deep insight from private document collections without ever sending data to the cloud.

---

## Features

### Elite RAG Pipeline
| Technique | What it does |
|---|---|
| **HyDE** (Hypothetical Document Embeddings) | Generates a hypothetical answer to bridge the semantic gap between your query and the source documents |
| **FlashRank Reranking** | Uses cross-encoders to re-score retrieved chunks, dramatically reducing hallucinations |
| **Semantic Chunking** | Splits documents on topic boundaries rather than fixed character counts |
| **GraphRAG** | Extracts entities and relationships into a Knowledge Graph for complex relational reasoning |

### Multi-Format Document Ingestion
- PDF — via PyPDF2
- DOCX — via python-docx
- Markdown & plain text

### Premium Interface
- **Glassmorphic dark UI** — a data-driven dashboard built with Streamlit
- **Live control panel** — toggle HyDE, Reranking, and Chunking strategies in real time
- **Source transparency** — inspect individual document chunks with relevance scores
- **Session persistence** — local history for seamless research continuity

---

## Tech Stack

| Layer | Technology |
|---|---|
| LLM Inference | Ollama (Llama 3, Mistral, Phi-3) |
| Vector Database | ChromaDB |
| Embeddings | Sentence-Transformers (`all-MiniLM-L6-v2`) |
| Reranker | FlashRank |
| Frontend | Streamlit |
| Language | Python 3.10+ |

---

## Getting Started

### Prerequisites
- [Ollama](https://ollama.ai) installed and running
- Python 3.10+
- At least one model pulled, e.g. `ollama pull llama3`

### Installation
```bash
# 1. Clone the repo
git clone https://github.com/YOUR_USERNAME/vantage.git
cd vantage

# 2. Create and activate a virtual environment
python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt
```

### Launch
```bash
streamlit run app.py
```

Then open `http://localhost:8501` in your browser.

---

## Usage

1. **Select a model** from the sidebar (any model you have pulled in Ollama)
2. **Upload documents** — drag and drop PDF, DOCX, or Markdown files and click **Index**
3. **Query** — use the chat interface with elite retrieval techniques active
4. **Inspect sources** — expand any response to see the exact chunks and relevance scores behind the answer

---

## Roadmap

- [ ] OCR support for scanned PDFs
- [ ] Multi-collection workspace management
- [ ] Export session as structured report
- [ ] REST API for headless integration
- [ ] LLM-generated Knowledge Graph visualizations

---

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.

---


<div align="center">
<sub>Built for those who keep their intelligence local.</sub>
</div>
