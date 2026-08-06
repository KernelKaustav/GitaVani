# GitaVani

**An AI-powered Speech Emotion Recognition system that recommends personalized Bhagavad Gita verses based on the user's emotional state.**

---

## Overview

GitaVani is an AI-based emotional wellness assistant that detects a user's emotional state directly from speech and recommends contextually relevant verses from the Bhagavad Gita, along with translations and practical interpretations.

The project combines Speech Emotion Recognition (SER), Deep Learning, and Natural Language Processing to provide personalized emotional and spiritual guidance.

Unlike traditional chatbot systems that rely solely on text, GitaVani understands emotions directly from speech.

---

## Objectives

- Detect emotions from speech using deep learning.
- Recommend contextually relevant Bhagavad Gita verses.
- Provide translations and practical interpretations.
- Develop an AI-powered emotional wellness assistant.
- Enable deployment for real-time embedded inference.

---

## System Pipeline

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
Translation and Interpretation
```

---

## Target Emotion Classes

| Emotion | Label |
|---------|------:|
| Calm | 0 |
| Joy | 1 |
| Sadness | 2 |
| Anger | 3 |
| Fear | 4 |

---

## Datasets

The model is trained using three publicly available Speech Emotion Recognition datasets.

| Dataset | Description |
|---------|-------------|
| RAVDESS | Ryerson Audio-Visual Database of Emotional Speech and Song |
| CREMA-D | Crowd-sourced Emotional Multimodal Actors Dataset |
| TESS | Toronto Emotional Speech Set |

The emotion labels from these datasets are unified into a common five-class taxonomy.

---

## Dataset Statistics

| Property | Value |
|----------|------:|
| Total Samples | 11,004 |
| Emotion Classes | 5 |
| Training Samples | 7,680 |
| Validation Samples | 1,624 |
| Test Samples | 1,700 |

---

## Repository Structure

```text
GitaVani
│
├── dataset
│   ├── raw
│   │   ├── ravdess
│   │   ├── crema-d
│   │   └── tess
│   │
│   └── processed
│       ├── audio
│       │   ├── train
│       │   ├── val
│       │   └── test
│       │
│       ├── metadata.csv
│       ├── train.csv
│       ├── val.csv
│       └── test.csv
│
├── notebook
│   ├── metadata.ipynb
│   ├── train-testsplit.ipynb
│   ├── audioprep.ipynb
│   ├── feature-extraction.ipynb
│   └── model-training.ipynb
│
├── outputs
├── src
├── tests
├── trained_model
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Machine Learning Pipeline

### Notebook 1 — Dataset Unification

- Load RAVDESS
- Load CREMA-D
- Load TESS
- Standardize emotion labels
- Create metadata.csv

**Output**

```
metadata.csv
```

---

### Notebook 2 — Dataset Splitting

- Speaker-aware train/validation/test split
- Preserve emotion distribution
- Prevent speaker leakage

**Output**

```
train.csv
val.csv
test.csv
```

---

### Notebook 3 — Audio Preprocessing

- Load audio
- Convert stereo to mono
- Resample to 16 kHz
- Standardize duration to 3 seconds
- Peak normalization
- Calm class augmentation
- Save processed audio

**Output**

```
processed/audio/
```

---

### Notebook 4 — Feature Extraction

- Short-Time Fourier Transform
- Mel Filter Bank
- Log-Mel Spectrogram generation
- Save NumPy feature tensors

**Output**

```
processed/mel/
```

---

### Notebook 5 — Model Training

- CNN architecture
- Weighted Cross Entropy Loss
- Model training
- Validation
- Testing
- Performance evaluation

**Output**

```
trained_model/
```

---

## Audio Preprocessing Pipeline

```text
Raw Audio
      │
      ▼
Mono Conversion
      │
      ▼
16 kHz Resampling
      │
      ▼
3 Second Standardization
      │
      ▼
Peak Normalization
      │
      ▼
Calm Class Augmentation
      │
      ▼
Processed Audio
```

---

## Feature Extraction Pipeline

```text
Processed Audio
      │
      ▼
Short-Time Fourier Transform
      │
      ▼
Mel Filter Bank
      │
      ▼
Log Scaling
      │
      ▼
Log-Mel Spectrogram
      │
      ▼
CNN Input
```

---

## Technologies

### Programming

- Python

### Machine Learning

- PyTorch
- Scikit-learn

### Audio Processing

- Librosa
- SoundFile
- Audiomentations

### Data Processing

- NumPy
- Pandas

### Visualization

- Matplotlib

### Development

- Jupyter Notebook
- Git
- GitHub

---

## Current Progress

| Component | Status |
|-----------|--------|
| Dataset Collection | Completed |
| Label Unification | Completed |
| Metadata Generation | Completed |
| Train/Validation/Test Split | Completed |
| Audio Preprocessing | Completed |
| Data Augmentation | Completed |
| Log-Mel Spectrogram Generation | In Progress |
| CNN Training | Planned |
| Model Evaluation | Planned |
| Bhagavad Gita Recommendation | Planned |
| Arduino Integration | Planned |
| Real-Time Inference | Planned |

---

## Future Work

- CNN-BiLSTM comparison
- Transformer-based Speech Emotion Recognition
- Sentence embedding-based verse retrieval
- Large Language Model explanations
- Text-to-Speech integration
- Edge AI optimization
- Raspberry Pi deployment
- Arduino deployment
- OLED display support
- Real-time microphone inference

---

## Expected Output

```text
Speech Input
      │
      ▼
Emotion Prediction
      │
      ▼
Bhagavad Gita Verse
      │
      ▼
Translation
      │
      ▼
Practical Interpretation
```

---

## License

This project is released under the MIT License.

---

## Author

**Kaustav Ghosh**

Artificial Intelligence • Deep Learning • Speech Emotion Recognition • Embedded AI
