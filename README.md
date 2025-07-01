# 🧠 Text Preprocessing in NLP — A Comparison using NLTK, SpaCy & Hugging Face

## 📌 Overview
This project explores and compares various text preprocessing techniques using three major NLP libraries:

- 🧰 **NLTK** – basic rule-based preprocessing  
- ⚙️ **SpaCy** – linguistically aware pipeline  
- 🤗 **Hugging Face** – subword-based tokenizer used in modern LLMs like BERT

We apply each pipeline to real-world Twitter data and analyze the tradeoffs through:

- Vocabulary compression  
- Token output comparison  
- Visualizations (top tokens, word clouds)  
- Use-case suitability analysis

---

## 🔍 Comparison Table

| Method           | Stopwords Removed | Lemmatized | Subwords | Notes                              |
|------------------|-------------------|------------|----------|------------------------------------|
| **NLTK**         | ✅ Yes            | ✅ Yes     | ❌ No    | Great for traditional ML models    |
| **SpaCy**        | ✅ Yes            | ✅ Yes     | ❌ No    | More linguistically accurate       |
| **Hugging Face** | ❌ No             | ❌ No      | ✅ Yes   | Keeps structure for LLMs like BERT |

---

## ✨ Highlights

- Cleaned **1,000 real tweets** from NLTK's Twitter dataset  
- Compared **vocabulary reduction** across pipelines  
- Visualized **top tokens & token distributions** by plotting token frequencies and word clouds to better understand what each method emphasizes.
- Showcased **different preprocessing strategies** for ML vs LLMs  

---

## 📌 Sample Token Output (Shortened View)

| Tweet # | NLTK Tokens                           | SpaCy Tokens                        | Hugging Face Tokens                            |
|--------|----------------------------------------|-------------------------------------|------------------------------------------------|
| #1     | `followfriday`, `top`, `engaged`,...   | `followfriday`, `engage`, `member` | `#`, `follow`, `##frid`, `##ay`, `@`, `france` |
| #2     | `hey`, `james`, `odd`, `call`,...      | `hey`, `james`, `odd`, `contact`   | `@`, `lamb`, `##2`, `##ja`, `hey`, `james`     |

> Full comparison table available in the notebook.

---

## 📁 Files

- `text_preprocessing_comparison.ipynb` – Full notebook with code, visualizations, and explanations  
- `README.md` – This file  

---

## 📚 How to Run

1. Clone the repo or download the notebook  
2. Install required libraries: `nltk`, `spacy`, `transformers`, `wordcloud`, `matplotlib`, etc.  
3. Run the notebook step-by-step

```bash
pip install nltk spacy transformers wordcloud matplotlib seaborn
python -m nltk.downloader all
python -m spacy download en_core_web_sm
```

## Author
Tarneem Alaa Abdelreheem - [LinkedIn](https://www.linkedin.com/in/tarneem-alaa-abdelreheem/) | [Github](https://github.com/TarneemAlaa1)
