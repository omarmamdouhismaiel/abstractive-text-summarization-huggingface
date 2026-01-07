# Abstractive Text Summarization with Hugging Face

This repository presents an end-to-end **abstractive text summarization** project using state-of-the-art Transformer models from **Hugging Face**.  
The project focuses not only on generating summaries, but also on **robust evaluation**, including semantic similarity, factual consistency, and performance analysis.

The implementation is designed for **research, experimentation, and portfolio demonstration**, following best practices used in real-world NLP workflows.

---

## Project Overview

- Apply pre-trained Transformer models for **abstractive summarization**
- Handle long documents using chunk-based summarization
- Evaluate summaries using multiple complementary metrics
- Analyze model behavior beyond ROUGE scores
- Provide reproducible and well-documented experimentation

---

## Models Used

- **BART** (`facebook/bart-large-cnn`)
- **PEGASUS** (`google/pegasus-cnn_dailymail`)
- **T5** (`t5-base`)

These models are widely used in industry and research for high-quality abstractive summarization.

---

## Evaluation Metrics

The project goes beyond basic evaluation by combining:

- **ROUGE-L** → Lexical overlap with reference summaries  
- **BERTScore (F1)** → Semantic similarity using contextual embeddings  
- **Hallucination Score** → Approximate factual consistency via NLI models  
- **Latency (seconds)** → Inference performance measurement  

This multi-metric evaluation provides a more realistic view of summarization quality.

---

## Repository Structure

abstractive-text-summarization-huggingface/  
├── huggingface_abstractive_summarization.ipynb  # Main notebook  
├── README.md                                    # Project documentation  
└── requirements.txt                             # Python dependencies  

---

## How to Run

### 1. Clone the repository
```bash
git clone https://github.com/your-username/abstractive-text-summarization-huggingface.git
cd abstractive-text-summarization-huggingface
```

### 2. Create a virtual environment (recommended)
```bash
python -m venv venv
source venv/bin/activate   # Linux / macOS
venv\Scripts\activate      # Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the notebook
Open the notebook in Jupyter or VS Code:
```bash
jupyter notebook huggingface_abstractive_summarization.ipynb
```

---

## Key Insights

- High **BERTScore F1** values indicate strong semantic alignment between generated summaries and references.
- Moderate **ROUGE-L** scores reflect the genuinely **abstractive** nature of the models.
- Most summaries remain **factually grounded**, with limited hallucination cases.
- Inference latency suggests the pipeline is best suited for **batch or offline summarization**.

---

## TL;DR

This project demonstrates a practical and evaluation-driven approach to **abstractive text summarization** using Hugging Face Transformers.  
It emphasizes **semantic quality, factual reliability, and performance considerations**, making it suitable for both learning and professional portfolio use.

---

## Future Improvements

- Fine-tuning models on domain-specific data
- Using long-context architectures (e.g. Long-T5, LED)
- Improving hallucination detection with sentence-level NLI batching
- Optimizing inference with batching or quantization
- Deploying the pipeline as an API (e.g. FastAPI)

---

## References

- Hugging Face Transformers: https://huggingface.co/docs/transformers  
- CNN/DailyMail Dataset: https://huggingface.co/datasets/cnn_dailymail  
- ROUGE Metric: https://aclanthology.org/W04-1013  
- BERTScore: https://arxiv.org/abs/1904.09675  

---

## Author

**Omar Mamdouh**  
Deep Learning & Generative AI Engineer

⭐ If you find this project useful, feel free to star the repository.

