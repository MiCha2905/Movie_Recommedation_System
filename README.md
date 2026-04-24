# 🎬 Conversational Movie Recommendation Chatbot

---

## 🧠 Overview
This project implements a **Conversational Movie Recommendation Chatbot** that suggests movies based on **natural language user queries**. Unlike traditional recommender systems, this chatbot allows users to interact in a human-like manner and receive personalized recommendations.

The system leverages **Natural Language Processing (NLP)** and a **content-based filtering approach** to provide relevant suggestions based on movie semantics.

---

## 🚀 Features
- 💬 Conversational interface for natural interaction  
- 🎯 Supports multiple query types:
  - Similar movies (e.g., *"movies like Inception"*)
  - Genre-based (e.g., *"action movies"*)
  - Rating-based (e.g., *"movies above rating 7"*)
- 🧠 Semantic recommendations using NLP  
- ⚡ Real-time responses  
- 📊 Clean and interpretable recommendation logic  

---

## 📂 Dataset
- Source: **TMDB (The Movie Database) API**
- Total Movies: **~300+**
- Features:
  - Title  
  - Year  
  - Genre  
  - Rating  
  - Overview (plot summary)  

---

## ⚙️ Methodology

### 1. Data Collection
- Movie data fetched using TMDB API  
- Multi-genre dataset for diversity  

### 2. Data Preprocessing
- Lowercasing text  
- Removing punctuation & stopwords  
- Handling missing values  
- Creating a **combined text feature** (title + genre + overview)

### 3. Feature Engineering
- **TF-IDF Vectorization** for text representation  
- Converts movie descriptions into numerical vectors  

### 4. Similarity Computation
- **Cosine Similarity** used to measure similarity between movies  
- Enables semantic matching instead of keyword-based matching  

### 5. Recommendation Engine
- 🎬 Similarity-based recommendations  
- 🎭 Genre-based filtering  
- ⭐ Rating-based filtering  

### 6. Conversational Logic
- Rule-based intent detection:
  - Similar movie queries  
  - Genre queries  
  - Rating queries  
- Routes user input to appropriate recommendation pipeline  

---

## 🤖 Example Queries
```text
"Recommend movies like The Godfather"
"Suggest action movies"
"Movies above rating 7"
