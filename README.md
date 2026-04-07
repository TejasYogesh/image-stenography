# 🖼️ Image Steganography using Python

A simple Python project that uses **Least Significant Bit (LSB) Steganography** to hide and extract secret text messages inside images.

---

## 📌 Table of Contents

- [🚀 Features](#-features)
- [🧠 How It Works](#-how-it-works)
- [📦 Setup Instructions](#-setup-instructions)
- [📄 Requirements](#-requirementstxt)
- [📁 Project Structure](#-project-structure)
- [▶️ Usage](#-usage)
- [⚠️ Important Notes](#️-important-notes)
- [🔒 Limitations](#-limitations)
- [💡 Future Improvements](#-future-improvements)
- [👨‍💻 Author](#-author)

---

## 🚀 Features

- 🔐 Encode secret messages into images  
- 🔍 Decode hidden messages from images  
- ⚡ Lightweight and efficient implementation  
- 🖼️ Supports common image formats like PNG and JPG  

---

## 🧠 How It Works

- Each pixel in an image contains RGB values.  
- This project modifies the **Least Significant Bit (LSB)** of the **Red channel**.  
- The message is converted into binary and stored bit-by-bit inside the image.  
- During decoding, these bits are extracted and converted back into text.  

---

## 📦 Setup Instructions

### 1️⃣ Create Virtual Environment

```bash
python -m venv venv
# Linux / Mac
source venv/bin/activate

# Windows
venv\Scripts\activate

# installation:
pip install -r requirements.txt


requirements.txt:
click==8.0.1
colorama==0.4.4
docopt==0.6.2
Flask==2.0.1
itsdangerous==2.0.1
Jinja2==3.0.1
MarkupSafe==2.0.1
numpy==1.20.3
opencv-python==4.5.2.52
Pillow==8.2.0
Werkzeug==2.0.1
