# 🌍 English-to-German LSTM Translator

This project implements a **Sequence-to-Sequence (Seq2Seq)** model with **LSTM** and **attention** to translate sentences from English to German. The model is trained on a tokenized dataset and evaluated using BLEU scores.

---

## 🧠 Architecture

- **Encoder:** Bidirectional LSTM  
- **Attention:** Bahdanau-style attention  
- **Decoder:** Unidirectional LSTM with attention context vector  
- **Loss Function:** CrossEntropyLoss 
- **Optimizer:** Adam  

---

## ⚙️ How It Works

1. **Tokenization** using basic rules or SpaCy.  
2. **Vocabulary** built from training data.  
3. **Training Loop**:  
   - Teacher forcing during training.  
   - Gradients clipped to avoid exploding gradients.  
4. **Evaluation**:  
   - BLEU score on the validation/test set.  
   - Translation of custom input sentences.  
