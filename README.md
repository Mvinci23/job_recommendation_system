# 🚀 Job Recommendation System using NLP

An end-to-end Machine Learning and NLP-based Job Recommendation System that suggests similar job roles based on job descriptions using TF-IDF and cosine similarity.

---

## 🧠 Project Overview

This project builds a job recommendation engine using Natural Language Processing (NLP) techniques. It analyzes job descriptions, titles, and positions to recommend similar jobs.

The system preprocesses text data, converts it into numerical features using TF-IDF vectorization, and computes similarity scores using cosine similarity to generate recommendations.

A Streamlit web application is developed to provide an interactive interface for users.

---

## 📂 Dataset

The dataset used in this project is sourced from Kaggle:

👉 https://www.kaggle.com/datasets/kandij/job-recommendation-datasets

### Dataset Features:
- Job Title  
- Company  
- Position  
- Job Description  
- Industry  
- Salary  

---

## 🔧 Data Preprocessing

The following NLP techniques were applied:

- Removed special characters using regex  
- Converted text to lowercase  
- Tokenization using NLTK  
- Stopword removal  
- Stemming using PorterStemmer  

Example transformation: 

Original: "Master piece of moving cat @9032"
Cleaned: "master piec move cat 9032"


---

## 🏗️ Feature Engineering

- Combined multiple columns:
  - Job Description  
  - Title  
  - Position  

- Created a new feature:

clean_text = Job.Description + Title + Position

🤖 Model Building

Used TF-IDF Vectorizer to convert text into numerical vectors

Computed similarity using Cosine Similarity

🎯 Recommendation System

The system recommends jobs using the following approach:

Select a job title

Find its index in dataset

Compute similarity scores

Sort jobs based on similarity

Return top similar jobs
