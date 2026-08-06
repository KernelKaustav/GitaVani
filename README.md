# 🕉️ GitaVani

> **An AI-powered Speech Emotion Recognition system that provides personalized Bhagavad Gita verses based on the user's emotional state.**

---

# 📖 Overview

GitaVani is an AI-powered emotional wellness assistant that detects a user's emotional state directly from their speech and recommends contextually relevant verses from the **Bhagavad Gita**, along with translations and practical interpretations.

The project combines **Speech Emotion Recognition (SER)**, **Deep Learning**, and **Natural Language Processing** to provide personalized spiritual guidance through voice interactions.

Unlike traditional chatbot systems, GitaVani understands **how a person feels**, rather than just **what they say**.

---

# 🎯 Objectives

- Detect emotions directly from speech using Deep Learning.
- Recommend contextually relevant Bhagavad Gita verses.
- Provide translation and practical interpretation of each verse.
- Build an AI-powered emotional wellness companion.
- Deploy the system for real-time inference using Arduino.

---

# 🏗️ System Pipeline

```text
                    User Speech
                         │
                         ▼
               Audio Preprocessing
                         │
                         ▼
               Feature Extraction
               (Log-Mel Spectrogram)
                         │
                         ▼
         CNN-based Speech Emotion Recognition
                         │
                         ▼
               Emotion Prediction
                         │
                         ▼
         Bhagavad Gita Verse Retrieval
                         │
                         ▼
      Translation + Practical Explanation
                         │
                         ▼
                Emotional Guidance
