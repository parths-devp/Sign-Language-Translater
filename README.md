# Sign-Language-Translater
# 🤟 ASL Sign Language to Speech using Deep Learning and Phi-3

An AI-powered Sign Language Recognition System that recognizes **American Sign Language (ASL)** alphabets from images using a **Convolutional Neural Network (CNN)**. The predicted text is refined using **Microsoft Phi-3** to generate a grammatically correct sentence, which is then converted into speech using **pyttsx3**.

---

## 📌 Features

- 🔤 Recognizes **29 ASL classes**
  - A–Z
  - Space
  - Delete
  - Nothing
- 🧠 CNN built using PyTorch
- 🤖 Grammar correction using Microsoft Phi-3
- 🔊 Offline Text-to-Speech using pyttsx3
- 🌐 Flask-based web application
- 💻 Terminal-based prediction support
- 📂 Supports prediction from multiple images

---

# 🛠 Tech Stack

- Python
- PyTorch
- TorchVision
- Hugging Face Transformers
- Microsoft Phi-3 Mini
- Flask
- Pillow (PIL)
- pyttsx3

---

# 📁 Project Structure

```text
PROJECTS/
│
├── sign_model.pth          # Trained CNN model
├── prediction.py           # Terminal prediction
├── grammar.py              # Phi-3 grammar correction
├── app.py                  # Flask web application
├── requirements.txt
├── README.md
├── ml_venv/
│
└── input_images/
    ├── 01.jpg
    ├── 02.jpg
    ├── 03.jpg
```

---

# 🧠 Model Architecture

The CNN consists of:

- 3 Convolution Layers
- Batch Normalization
- ReLU Activation
- Max Pooling
- Adaptive Average Pooling
- Fully Connected Layers
- Dropout Regularization

The model predicts **29 classes**:

```text
A-Z
space
del
nothing
```

---

# ⚙️ Workflow

```text
Input Images
      │
      ▼
Image Preprocessing
      │
      ▼
CNN Prediction
      │
      ▼
Predicted Letters
      │
      ▼
Form Text
      │
      ▼
Phi-3 Grammar Correction
      │
      ▼
Text-to-Speech
```

---

# 🚀 Installation

## Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/ASL-Sign-Language-To-Speech.git

cd ASL-Sign-Language-To-Speech
```

---

## Create Virtual Environment

### Windows

```bash
python -m venv ml_venv
```

Activate

```bash
ml_venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv ml_venv

source ml_venv/bin/activate
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Running the Project

## Terminal Version

Place your images inside:

```text
input_images/
```

Run:

```bash
python prediction.py
```

Example Output:

```text
01.jpg -> I
02.jpg -> space
03.jpg -> H
04.jpg -> A
05.jpg -> P
06.jpg -> P
07.jpg -> Y

CNN Output:
I HAPPY

LLM Output:
I am happy.
```

The computer will then speak:

```text
I am happy.
```

---

## Flask Web Application

Run:

```bash
python app.py
```

Open your browser:

```text
http://127.0.0.1:5000
```

Upload an ASL image to receive:

- Predicted Letter
- Raw Text
- Grammar Corrected Sentence

---

# 📊 Example Pipeline

```text
Input Images
      │
      ▼
CNN
      │
      ▼
Predicted Letters

I
space
H
A
P
P
Y

      │
      ▼
I HAPPY

      │
      ▼
Microsoft Phi-3

"I am happy."

      │
      ▼
Text-to-Speech
```

---

# 📦 Dataset

The project uses the **ASL Alphabet Dataset**, containing **29 classes**:

- A–Z
- space
- del
- nothing

---

# 🔮 Future Improvements

- Real-time webcam prediction
- Word-level sign language recognition
- Sentence-level prediction
- Confidence score visualization
- Support for additional sign languages
- Audio playback controls
- Model optimization for edge devices

---

# 👨‍💻 Author

**Vedika Panurkar**

B.Tech Robotics and Automation  
Walchand College of Engineering, Sangli

GitHub: https://github.com/vedikapanurkar16-sys

---
