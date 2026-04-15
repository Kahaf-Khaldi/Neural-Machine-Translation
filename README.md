# Neural Machine Translation using Encoder-Decoder (Seq2Seq)

## Overview
This project implements a **Neural Machine Translation (NMT)** system using a **Sequence-to-Sequence (Seq2Seq) Encoder-Decoder architecture**. The model learns to translate text from a **source language to a target language** using deep learning techniques.

Unlike traditional rule-based or statistical approaches, this model leverages **LSTM-based neural networks** to understand and generate language sequences effectively.

---

## Model Architecture

The system is based on the Encoder-Decoder framework:

Input Sentence → Encoder (LSTM) → Context Vector → Decoder (LSTM) → Output Sentence

### 🔹 Encoder
- Processes input sequence  
- Encodes it into a fixed-length context vector  

### 🔹 Decoder
- Takes context vector as input  
- Generates translated sequence step-by-step  

---

## ⚙️ Tech Stack

- Python
- TensorFlow / Keras 🤖  
- NumPy  
- Pandas  
- Natural Language Processing (NLP)

---

---

## 📊 Dataset

- Parallel corpus (source ↔ target language pairs)

Example:

English → French  
Hello → Bonjour  
How are you? → Comment ça va ?

---

## 🔄 Workflow

### 1. Data Preprocessing
- Lowercasing  
- Tokenization  
- Padding sequences  
- Vocabulary indexing  

### 2. Model Building
- Encoder LSTM  
- Decoder LSTM  
- Dense + Softmax output layer  

### 3. Training
- Loss Function: `categorical_crossentropy`  
- Optimizer: `Adam`  
- Technique: Teacher Forcing  

### 4. Inference
- Generate translations word-by-word  
- Uses trained encoder & decoder models  

---

## 📈 Results

The Neural Machine Translation model was successfully trained using the Encoder-Decoder (Seq2Seq) architecture.

### 🔹 Model Performance
- The model is able to generate meaningful translations for simple and medium-length sentences  
- Handles variable-length input and output sequences effectively  
- Learns contextual relationships between words using LSTM networks  

### 🔹 Sample Predictions

| Input Sentence | Predicted Translation |
|---------------|---------------------|
| Hello         | Bonjour             |
| How are you?  | Comment ça va ?     |
| I am fine     | Je vais bien        |
| Thank you     | Merci               |

### 🔹 Observations
- The model performs well on frequently seen sentence patterns  
- Translation quality decreases for:
  - Long sentences  
  - Rare or unseen words  

### 🔹 Limitations
- No attention mechanism (context bottleneck issue)  
- Limited vocabulary size  
- Basic Seq2Seq architecture  

### 🔹 Evaluation (Optional Metrics)
- Accuracy improves with training epochs  
- Can be further evaluated using:
  - BLEU Score  
  - Perplexity  

---
