# Face Recognition & OCR System

A Python-based computer vision project that combines **face recognition** and **OCR (Optical Character Recognition)** to process images or video using a webcam/camera.

The project uses OpenCV for image processing, `face_recognition` for identifying faces, and Tesseract OCR for extracting text from images. Recognition or processing results can also be recorded with timestamps in CSV format.

## 🚀 Features

* 📷 Image/video processing using OpenCV
* 👤 Face detection and face recognition
* 🔤 Optical Character Recognition (OCR) using Tesseract
* 🧮 Numerical processing using NumPy
* ⏰ Timestamp generation using Python `datetime`
* 📄 CSV-based data/result logging
* 📁 File and directory management using `os`

## 🛠️ Technologies & Libraries

| Library                 | Purpose                                       |
| ----------------------- | --------------------------------------------- |
| `opencv-python` (`cv2`) | Image and video processing                    |
| `pytesseract`           | Extracts text from images using Tesseract OCR |
| `face-recognition`      | Face detection and face recognition           |
| `numpy`                 | Numerical and array operations                |
| `datetime`              | Date and time handling                        |
| `csv`                   | Reading and writing CSV files                 |
| `os`                    | File and directory management                 |

## 📦 Installation

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
cd YOUR_REPOSITORY
```

### 2. Create a virtual environment

It is recommended to use a virtual environment.

**Windows:**

```bash
python -m venv venv
venv\Scripts\activate
```

**Linux / macOS:**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Python dependencies

```bash
pip install opencv-python pytesseract face-recognition numpy
```

The `os`, `datetime`, and `csv` modules are part of Python's standard library, so they do not need to be installed separately.

## 🔤 Tesseract OCR Setup

`pytesseract` is a Python wrapper for the **Tesseract OCR engine**, so Tesseract itself must also be installed on your computer.

After installing Tesseract, make sure it is available to your system or configure its path in your Python code.

Example for Windows:

```python
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"
```

The exact path may differ depending on where Tesseract is installed.

## ▶️ Running the Project

Activate your virtual environment and run your Python program:

```bash
python main.py
```

Replace `main.py` with the actual name of your Python file.

## 📂 Example Project Structure

```text
project/
│
├── main.py
├── images/
│   ├── person1.jpg
│   └── person2.jpg
│
├── output/
│   └── results.csv
│
├── requirements.txt
├── .gitignore
└── README.md
```

## 📋 Requirements

Create a `requirements.txt` file containing:

```text
opencv-python
pytesseract
face-recognition
numpy
```

Then dependencies can be installed with:

```bash
pip install -r requirements.txt
```

## ⚠️ Notes

* A working camera/webcam may be required depending on how the project is implemented.
* Tesseract OCR must be installed separately from the Python `pytesseract` package.
* The `face-recognition` library may require additional dependencies depending on your operating system and Python version.
* Make sure you have permission to process and store biometric or personal data when using face recognition.

## 🔒 Privacy

Face recognition involves biometric information. Use this project responsibly and ensure that you have appropriate consent and authorization when processing people's faces or personal information.

## 📄 License

Add an appropriate license to this project if you plan to distribute or publish it.

---

## 👨‍💻 Author

**Your Name**

GitHub: `https://github.com/YOUR_USERNAME`
