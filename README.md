# 🌐 Neural Machine Translation using Seq2Seq (Encoder-Decoder)

![Python](https://img.shields.io/badge/Python-3.9-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-DeepLearning-orange)
![NLP](https://img.shields.io/badge/Domain-NLP-green)
![Status](https://img.shields.io/badge/Project-Completed-success)

---

## 📌 Overview

This project implements a **Neural Machine Translation (NMT)** system using a **Sequence-to-Sequence (Seq2Seq) Encoder-Decoder architecture** with LSTM networks.

The model learns to translate sentences from a **source language to a target language** by capturing contextual dependencies in sequential data.

Unlike traditional statistical methods, this approach leverages **deep learning to generate more natural and context-aware translations**.

---

## 🧠 Architecture

The model is based on the Seq2Seq framework:

Input Sentence → Encoder (LSTM) → Context Vector → Decoder (LSTM) → Output Sentence

### 🔹 Encoder
- Encodes input sequence into context vector  
- Captures semantic meaning of the sentence  

### 🔹 Decoder
- Generates translated output step-by-step  
- Uses previous outputs as input  

---

## ⚙️ Tech Stack

- Python  
- TensorFlow / Keras  
- NumPy  
- Pandas  
- NLP Techniques  

---

---

## 🔄 Workflow

### 1️⃣ Data Preprocessing
- Text cleaning & normalization  
- Tokenization  
- Padding sequences  
- Vocabulary creation  

### 2️⃣ Model Building
- Encoder (LSTM)  
- Decoder (LSTM)  
- Dense + Softmax layer  

### 3️⃣ Training
- Loss: `categorical_crossentropy`  
- Optimizer: `Adam`  
- Technique: Teacher Forcing  

### 4️⃣ Inference
- Generate translations word-by-word  
- Separate encoder-decoder models for prediction  

---

## 📈 Results

### 🔹 Model Performance
- Successfully translates basic and intermediate sentences  
- Learns contextual relationships between words  
- Handles variable-length sequences  

### 🔹 Sample Predictions

| Input Sentence | Predicted Translation |
|---------------|---------------------|
| Hello         | Bonjour             |
| How are you?  | Comment ça va ?     |
| I am fine     | Je vais bien        |
| Thank you     | Merci               |

### 🔹 Observations
- Performs well on common sentence structures  
- Struggles with long or rare sequences  

### 🔹 Limitations
- No attention mechanism (information bottleneck)  
- Limited vocabulary coverage  

---


