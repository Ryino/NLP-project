# Urdu-English Neural Machine Translation (NMT)

This project implements a high-performance Transformer-based Neural Machine Translation (NMT) system for translating between Urdu and English using TensorFlow and FastText embeddings. The system supports custom preprocessing, vocabulary building, tokenization, and training workflows.

---

## 🚀 Key Improvements Made

### ✅ Optimized Tokenization
- Integrated lightweight `spacy.blank` tokenizers instead of loading large models.
- Fallback tokenization provided for robustness.
- Automatic truncation and warning for long sequences.

### ✅ Robust Data Handling
- Improved dataset loading with line limits and encoding checks.
- Train/Validation/Test splits implemented for reproducibility.
- Input validation and exception handling added.

### ✅ FastText Embeddings
- Supports pre-trained FastText vectors for both English and Urdu.
- Embedding matrices are efficiently constructed and cached.
- Automatically handles out-of-vocabulary (OOV) words.

### ✅ Transformer Architecture
- Modular and clean TensorFlow Keras subclass model.
- Supports pretrained embeddings with frozen weights.
- Custom positional encoding and multi-head attention.
- Decoder/Encoder layering follows best practices for NMT.

### ✅ Logging and Debugging
- Informative logging throughout all steps (data loading, tokenization, vocab building, training).
- Warns of slow operations, input anomalies, and fallback modes.

---

## ⚙️ Technologies Used

- **TensorFlow 2.x**
- **Spacy (Lightweight Tokenization)**
- **FastText (Embeddings)**
- **NumPy / Pandas / Scikit-learn**
- **Python 3.8+**

---


Ensure:
- UTF-8 encoding.
- Sentence length ≤ 500 characters.
- Same number of lines in both files.

---

## 🛠️ How to Run

### 1. Install Dependencies

```bash
pip install tensorflow spacy fasttext pandas scikit-learn
python -m spacy download en_core_web_sm
```

## 🛠️ Authors

Rayyan Hassan(2021535) and Faakhir Inam (2021152)



