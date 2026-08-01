# 🕉️ GitaVani

> **An AI-powered Speech Emotion Recognition system that provides personalized Bhagavad Gita verses based on the user's emotional state.**

![Python](https://img.shields.io/badge/Python-3.12-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red)
![Status](https://img.shields.io/badge/Status-Under%20Development-orange)
![License](https://img.shields.io/badge/License-MIT-green)

---

# 📖 Overview

GitaVani is an AI-based emotional wellness assistant that analyzes a user's speech to detect emotions and recommends relevant verses from the **Bhagavad Gita** along with their meaning and practical guidance.

The project combines **Speech Emotion Recognition (SER)** with **Natural Language Processing** to provide personalized spiritual and emotional support.

Instead of relying on text input, GitaVani understands **human emotions directly from voice**.

---

# 🎯 Objectives

- Detect emotions from speech using Deep Learning.
- Recommend contextually relevant Bhagavad Gita verses.
- Provide translation and practical interpretation.
- Build an AI-powered emotional wellness companion.

---

# 🏗️ Project Pipeline

```
User Speech
      │
      ▼
Audio Preprocessing
      │
      ▼
Feature Extraction
(Mel Spectrogram)
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
Translation + Explanation
```

---

# 🎭 Target Emotions

The model classifies speech into five emotions:

| Emotion | Label |
|----------|------:|
| Calm | 0 |
| Joy | 1 |
| Sadness | 2 |
| Anger | 3 |
| Fear | 4 |

---

# 📂 Datasets Used

The project combines three public Speech Emotion Recognition datasets.

| Dataset | Description |
|----------|-------------|
| RAVDESS | Ryerson Audio-Visual Database of Emotional Speech and Song |
| CREMA-D | Crowd-sourced Emotional Multimodal Actors Dataset |
| TESS | Toronto Emotional Speech Set |

All datasets are unified into a common five-class emotion taxonomy.

---

# 📁 Repository Structure

```
GitaVani
│
├── dataset
│   ├── raw
│   └── processed
│       ├── metadata.csv
│       ├── train.csv
│       ├── val.csv
│       └── test.csv
│
├── notebook
│   ├── metadata.ipynb
│   └── train-testsplit.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

# 🛠️ Current Progress

- [x] Downloaded and organized datasets
- [x] Unified emotion labels across datasets
- [x] Created metadata.csv
- [x] Generated train/validation/test splits
- [ ] Audio preprocessing
- [ ] Data augmentation
- [ ] Mel Spectrogram generation
- [ ] CNN model training
- [ ] Emotion prediction
- [ ] Bhagavad Gita recommendation engine
- [ ] Arduino integration
- [ ] Real-time inference

---

# 🔬 Machine Learning Pipeline

## Notebook 1
Dataset unification

- Merge RAVDESS, CREMA-D and TESS
- Standardize emotion labels
- Create metadata.csv

## Notebook 2
Dataset splitting

- Speaker-aware train/validation/test split
- Preserve emotion distribution
- Generate train.csv, val.csv and test.csv

## Notebook 3
Audio preprocessing

- Resampling
- Normalization
- Fixed duration
- Data augmentation

## Notebook 4
Feature extraction

- Mel Spectrogram generation
- Save processed features

## Notebook 5
Model training

- CNN architecture
- Weighted Cross Entropy Loss
- Model evaluation

---

# 🚀 Technologies

- Python
- PyTorch
- NumPy
- Pandas
- Librosa
- Scikit-learn
- Jupyter Notebook
- Matplotlib

---

# 📊 Future Enhancements

- CNN + BiLSTM comparison
- Transformer-based Speech Emotion Recognition
- Sentence-Embedding based Gita verse retrieval
- Text-to-Speech integration
- Real-time microphone inference
- Raspberry Pi deployment
- Arduino integration
- OLED display support

---

# 🤝 Contributing

Contributions are welcome.

Feel free to open issues or submit pull requests.

---

# 📜 License

This project is released under the MIT License.

---

# 👨‍💻 Author

**Kaustav Ghosh**

AI | Deep Learning | Computer Vision | Speech Emotion Recognition
