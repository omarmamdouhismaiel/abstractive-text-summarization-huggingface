# Abstractive Text Summarization with Hugging Face

**Portfolio Project by Omar Mamdouh**

This project demonstrates **abstractive text summarization** using Hugging Face Transformers. It compares **BART, PEGASUS, and T5** models on the **CNN/DailyMail dataset** and evaluates them using **ROUGE metrics** and **qualitative analysis**.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Models](#models)
4. [Evaluation](#evaluation)
5. [Key Insights](#key-insights)
6. [Skills Demonstrated](#skills-demonstrated)
7. [Limitations & Future Work](#limitations--future-work)
8. [How to Run](#how-to-run)
9. [Author](#author)
10. [License](#license)
11. [Acknowledgements](#acknowledgements)

---

## Project Overview
The goal is to generate concise, human-like summaries from news articles while preserving the main information. This project provides a full **end-to-end pipeline** including:

- Dataset loading
- Model inference
- Automatic evaluation (ROUGE)
- Hyperparameter experimentation (beam search)
- Qualitative inspection of summaries
- Model selection

---

## Dataset
- **Dataset:** CNN/DailyMail (v3.0.0)  
- **Type:** News articles with human-written highlights  
- **Subset Used:** First 100 test samples for faster evaluation  
- **Columns:** `article` (input), `highlights` (reference summary)

---

## Models
Three Hugging Face transformer models were compared:

| Model    | Description |
|----------|-------------|
| BART     | Fluent, human-like summaries, widely used in summarization tasks |
| PEGASUS  | Concise summaries, optimized for news datasets |
| T5       | Lightweight, flexible for multi-task NLP, may produce shorter summaries |

---

## Evaluation
- **ROUGE Metrics:** ROUGE-1, ROUGE-2, ROUGE-L for automatic evaluation  
- **Qualitative Analysis:** Sample summaries inspected for coherence, completeness, and human-like readability  
- **Hyperparameter Experiments:** Beam search to improve summary fluency

---

## Key Insights
- **BART** provides the most fluent and coherent summaries overall  
- **PEGASUS** is concise, may omit minor details  
- **T5** is lightweight but less consistent on longer articles  
- Hyperparameter tuning improves fluency but slows inference  
- ROUGE scores align with qualitative evaluation

---

## Skills Demonstrated
- NLP & Transformer Models (Hugging Face pipelines)  
- Model evaluation (ROUGE metrics, qualitative analysis)  
- Python data handling (Pandas, Matplotlib)  
- End-to-end **portfolio-ready project presentation**

---

## Limitations & Future Work
**Limitations:**
- ROUGE does not fully capture semantic correctness  
- Models may hallucinate facts  
- Dataset limited to news articles  

**Future Work:**
- Fine-tune models on domain-specific datasets  
- Use semantic evaluation metrics (BERTScore)  
- Handle long documents with chunking  
- Deploy as web service (FastAPI / Streamlit)

---

## How to Run

1. **Clone the repository**:

```
git clone https://github.com/YourUsername/abstractive-text-summarization-huggingface.git
```

2. **Install requirements**:

```
pip install -r requirements.txt
```

3. **Run the notebook**:
- Open `Abstractive_Text_Summarization.ipynb` in Jupyter Notebook or Kaggle.

4. **View Results**:
- Automatic evaluation metrics (ROUGE-1, ROUGE-2, ROUGE-L)
- Qualitative summary comparison tables
- ROUGE visualizations and insights

---

## Author

**Omar Mamdouh**  

- LinkedIn: [[LinkedIn profile](https://www.linkedin.com/in/omar-mamdouh-ismaiel/)]  
- GitHub: [[GitHub Profile](https://github.com/omarmamdouhismaiel)]  

---

## License

This project is open-source and available under the **MIT License**.  
Feel free to use, modify, and share for educational and portfolio purposes.

---

## Acknowledgements

- Hugging Face Transformers: https://huggingface.co/transformers/  
- CNN/DailyMail Dataset: https://huggingface.co/datasets/cnn_dailymail  
- Evaluate Library (ROUGE metrics): https://huggingface.co/docs/evaluate/index
