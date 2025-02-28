# Hand Gesture-Based LED Control

## 🚀 Getting Started

This project allows you to control LEDs using hand gestures through computer vision and an Arduino board.

---

## 🛠 Prerequisites

Ensure you have the following installed before running the project:

### 1️⃣ Install Python (If Not Installed)
Check if Python (version **3.7+** recommended) is installed:
```sh
python --version
```
If not installed, [Download Python](https://www.python.org/downloads/).

### 2️⃣ Install Required Libraries
Run the following command to install the necessary dependencies:
```sh
pip install opencv-python cvzone pyfirmata2
```
⚠ If you face OpenCV issues, try:
```sh
pip install opencv-python-headless
```

### 3️⃣ Install MediaPipe (For Hand Tracking)
Since **cvzone** uses **MediaPipe**, install it using:
```sh
pip install mediapipe
```

### 4️⃣ Setup Arduino (For LED Control)
If you're using an **Arduino** board, install the required library:
```sh
pip install pyfirmata2
```
- Connect your Arduino via **USB**.
- Find your **COM port**:
  - **Windows**: Open *Device Manager* → *Ports*.
  - **Mac/Linux**: Use `ls /dev/tty*` to find the correct port.
- Update `controller.py`:
```python
comport = 'COM10'  # Replace with your actual COM port
```

---

## ▶ Running the Project
Once everything is set up, execute the script:
```sh
python your_script.py
```

### 🎥 Camera Issues?
- Ensure your **webcam permissions** are enabled.
- If your laptop has multiple cameras, modify the video index:
```python
video = cv2.VideoCapture(1)  # Change 1 to 0 or 2 if needed
```

---

## 🔧 Troubleshooting
### ❌ "No module named cvzone" error?
Try reinstalling:
```sh
pip install --upgrade cvzone
```

### 📷 Camera doesn't open?
- Ensure no other applications are using the webcam.
- Restart your system and try again.

---

## 🤝 Contributing
Feel free to fork this repository and improve the project. Pull requests are welcome!

---

## 📩 Contact
For any queries, reach out via [GitHub Issues](https://github.com/raviranjan-star/Hand-Gesture-Based-LED-Control/issues).

**Happy Coding! 🚀**

