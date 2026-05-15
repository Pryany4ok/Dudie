
# 📸 Features

- Real-time hand tracking
- Gesture recognition using MediaPipe
- Video playback control with gestures
- Webcam integration
- Lightweight and simple setup
- Cross-platform support (Linux / Windows / macOS)

---

# ⚠️ IMPORTANT PYTHON VERSION NOTE

This project **MUST** be executed using:

```text
Python 3.10.x
```

The project is **NOT guaranteed to work** with:

- Python 3.11+
- Python 3.9 or lower

This is due to compatibility issues with **MediaPipe** and some OpenCV dependencies.

---

# 🛠️ Requirements

## Software

- Python 3.10.x
- pip
- virtualenv (recommended)

## Python Libraries

- OpenCV
- MediaPipe
- NumPy

## Hardware

- Webcam
- `gato.mp4` video file in the root directory

---

# 📂 Project Structure

```text
Scubacat/
│
├── scubacat.py
├── gato.mp4
├── requirements.txt
└── README.md
```

---

# 🚀 Installation & Setup

## 1. Clone the repository

```bash
git clone https://github.com/Pryany4ok/Dudie.git
cd Scubacat
```

---

## 2. Create a virtual environment

Using a virtual environment is strongly recommended.

### Linux / macOS

```bash
python3.10 -m venv .venv
source .venv/bin/activate
```
(fish)
```bash
python3.10 -m venv .venv
source .venv/bin/activate.fish
```

### Windows

```bash
python -m venv .venv
.venv\Scripts\activate
```

---

## 3. Upgrade pip

```bash
python -m pip install --upgrade pip
```

---

## 4. Install dependencies

```bash
pip install -r requirements.txt
```

Or manually:

```bash
pip install opencv-python mediapipe numpy
```

---

# ▶️ Running The Project

Make sure:

- Your webcam is connected
- `gato.mp4` exists in the same folder as `scubacat.py`

Then run:

```bash
python scubacat.py
```

---

# ✋ Gesture Logic

The application detects and tracks hand landmarks using MediaPipe.

## ✊ Fist Gesture

When the fingertips move close to the palm base:

✅ The cat video starts playing automatically.

---

## 🖐️ Open Palm Gesture

When all fingers are extended:

✅ The video stops and the playback window closes.

---

## ⎋ ESC Key

Pressing the ESC key:

✅ Stops the webcam capture  
✅ Closes all windows  
✅ Terminates the program

---

# 🧠 Technologies Used

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| OpenCV | Video capture and rendering |
| MediaPipe | Hand tracking and gesture detection |
| NumPy | Array and numerical operations |

---

# 🐧 Linux Notes

On Linux distributions like:

- Arch Linux
- CachyOS
- EndeavourOS
- Fedora
- Ubuntu

you may need to explicitly use Python 3.10:

```bash
python3.10 scubacat.py
```

---

# 🛑 Troubleshooting

## ❌ `AttributeError: module 'mediapipe' has no attribute 'solutions'`

Possible causes:

### 1. Wrong Python version

Check your Python version:

```bash
python --version
```

You MUST use:

```text
Python 3.10.x
```

---

### 2. Local file conflict

Make sure your project folder does NOT contain:

```text
mediapipe.py
```

or:

```text
mediapipe/
```

These names conflict with the official MediaPipe package.

---

## ❌ Webcam does not open

Make sure no other applications are using the webcam:

- Discord
- Zoom
- Teams
- OBS
- Browser camera access

---

## ❌ Video does not play

Verify:

- `gato.mp4` exists
- File name is exactly correct
- Video codec is supported by OpenCV

---

## ❌ `pip` command not found

Try:

```bash
python -m pip install --upgrade pip
```

---

# 📦 requirements.txt Example

```txt
opencv-python
mediapipe
numpy
```

---

# 💡 Recommended Setup

Recommended environment:

| Component | Version |
|---|---|
| Python | 3.10.x |
| OpenCV | Latest |
| MediaPipe | 0.10.x |
| OS | Linux / Windows |

---


# 👨‍💻 Author

[mishuka
](https://github.com/mishu006)
---

# ⭐ Support

If you like this project:

- Give the repository a star ⭐
- Fork the project 🍴
- Contribute improvements 🚀

---
