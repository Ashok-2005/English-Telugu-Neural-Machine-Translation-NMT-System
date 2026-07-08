# Regional Language Translator – English to Telugu

An English-to-Telugu Neural Machine Translation (NMT) system developed using deep learning techniques. This project explores both a custom Seq2Seq with Attention model and Transformer-based translation models, along with transfer learning using a pretrained Helsinki-NLP model.

---

## 📌 Overview

This project aims to bridge the language gap between English and Telugu by developing an intelligent Neural Machine Translation (NMT) system. Telugu is a morphologically rich language with flexible word order, making traditional rule-based translation difficult.

The project investigates multiple translation approaches:

- Seq2Seq with Bahdanau Attention
- Transformer-based Neural Machine Translation
- Fine-tuned Helsinki-NLP pretrained translation model (used for cross-validation)

The models were evaluated using BLEU and chrF metrics to measure translation quality.

---

## 🎯 Objectives

- Develop an English-to-Telugu Neural Machine Translation system.
- Compare Seq2Seq and Transformer architectures.
- Handle Telugu morphology using subword tokenization.
- Improve translation quality using pretrained language models.
- Evaluate performance using BLEU and chrF metrics.
- Build a simple web interface for real-time translation.

---

## ✨ Features

- English → Telugu translation
- Seq2Seq with Attention implementation
- Transformer-based translation
- Transfer learning using Helsinki-NLP model
- Parallel corpus preprocessing
- Byte Pair Encoding (BPE) tokenization
- BLEU and chrF evaluation
- 5-Fold Cross Validation
- Web-based translation interface

---

# 🛠️ Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- TensorFlow / Keras
- SentencePiece
- NumPy
- Pandas

---

# 📂 Dataset

The parallel English–Telugu corpus was created using publicly available bilingual datasets and text sources, including:

- Samanantar
- OPUS
- Wikipedia
- News Articles
- Government Documents
- Public Parallel Corpora

### Data Preprocessing

- Text cleaning
- Unicode normalization
- Tokenization
- Byte Pair Encoding (BPE)
- Padding & masking
- Train / Validation / Test split

---

# 🧠 Models Implemented

## 1. Seq2Seq with Attention

- Bidirectional LSTM Encoder
- LSTM Decoder
- Bahdanau Attention
- Teacher Forcing
- Beam Search Decoding

---

## 2. Transformer Model

A Transformer-based Neural Machine Translation model was implemented and evaluated for English-to-Telugu translation.

---

## 3. Fine-Tuned Helsinki-NLP Model

For model robustness evaluation, the pretrained **Helsinki-NLP/opus-mt-en-dra** model was fine-tuned on the custom English–Telugu dataset and evaluated using **5-fold cross-validation**.

> **Note:** The fine-tuned Helsinki-NLP model was used only for the cross-validation experiment.

---

# 📊 Evaluation Metrics

The models were evaluated using:

- BLEU Score
- chrF Score
- 5-Fold Cross Validation

---

# 📈 Results

## Transformer Model

| Metric | Trained | New Test |
|--------|---------:|---------:|
| BLEU | 0.16 | 0.13 |
| chrF | 12.64 | 5.72 |

---

## Seq2Seq with Attention

| Metric | Trained | New Test |
|--------|---------:|---------:|
| BLEU | 22.21 | 0.23 |
| chrF | 55.22 | 12.70 |

---

## 5-Fold Cross Validation (Fine-Tuned Helsinki-NLP Model)

| Metric | Fold-1 | Fold-2 | Fold-3 | Fold-4 | Fold-5 |
|--------|-------:|-------:|-------:|-------:|-------:|
| BLEU | 63.3697 | 63.2564 | 63.1482 | 63.1887 | 63.5662 |
| chrF | 82.1624 | 82.1292 | 82.0905 | 82.1032 | 82.2937 |

### Average Cross-Validation Performance

| Metric | Score |
|--------|------:|
| BLEU | **63.31** |
| chrF | **82.16** |

---

# 💻 Sample Translation

**Input**

```
He is reading a book which was given by his friend.
```

**Output**

```
అతను తన స్నేహితుడు ఇచ్చిన ఒక పుస్తకం చదువుతున్నాడు.
```

---

# 📌 Key Contributions

- Developed an English-to-Telugu Neural Machine Translation system.
- Implemented a Seq2Seq model with Bahdanau Attention.
- Implemented a Transformer-based translation model.
- Fine-tuned the Helsinki-NLP pretrained translation model for cross-validation.
- Evaluated translation quality using BLEU and chrF metrics.
- Developed a web interface for real-time translation.

---

# 🔮 Future Work

- Support bidirectional translation (Telugu ↔ English).
- Fine-tune larger multilingual models such as IndicTrans2 and mBART.
- Increase the size and diversity of the parallel corpus.
- Improve translation quality for long and domain-specific sentences.
- Deploy the model as a REST API and mobile application.
- Integrate speech-to-text and text-to-speech modules.

---

# 👨‍💻 Authors

- **Venkata Ashok Adithya**
- **Harshavardhan Reddy**
- **Dinesh Reddy**
- **Kaseeswar**
**School of Computer Science and Engineering**

**VIT-AP University**

---

# 📚 References

- Vaswani et al., *Attention Is All You Need* (2017)
- Helsinki-NLP OPUS-MT Models
- Hugging Face Transformers
- Samanantar Dataset
- OPUS Parallel Corpus
