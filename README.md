# 🛠️ PPE Detection Project

## 🚀 Overview
This project implements a **Personal Protective Equipment (PPE) Detection System** designed to ensure workplace safety by identifying whether individuals are wearing the required safety gear. Using deep learning, the system evaluates real-time video feeds or images to detect vests, helmets (yellow, white, or blue), and their combinations to classify individuals as 'safe' or 'unsafe'.

---

## 🧠 Features

- 🎥 **Real-Time Detection**: Processes live video streams or webcam feeds.
- 🦺 **Safety Gear Identification**: Detects vests and helmets.
- ✅ **Safety Classification**:
  - Person wearing a vest and any of the specified helmet colors is classified as **Safe**.
  - Missing either vest or helmet is classified as **Unsafe**.
- 🤖 **Deep Learning Model**: Uses a trained **YOLO model** for object detection.

---

## 🛠️ Technologies Used

- **Programming Language**: Python 🐍
- **Deep Learning Framework**: YOLO (You Only Look Once)
- **Webcam Integration**: OpenCV 📷
- **Real-Time Classification**: TensorFlow/Keras for supplementary classification.

---

## ⚙️ How It Works
1. **Object Detection**:
   - YOLO model identifies objects in the frame (e.g., `person`, `vest`, `helmet`).
2. **Classification Logic**:
   - If a `person` and `vest` are detected, along with any helmet color (yellow, white, blue), the individual is marked as **Safe**.
   - Otherwise, they are classified as **Unsafe**.
3. **Output Display**:
   - The system overlays the detection results on the video feed.

---

## 🧑‍💻 Setup & Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/ppe-detection.git
   cd ppe-detection
   ```

2. **Install Requirements**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Application**:
   ```bash
   python app.py
   ```

4. **Use the Webcam**:
   Ensure the system has access to the webcam for real-time detection.

---

## 📂 Directory Structure

```
.
├── models/           # Pre-trained YOLO and Keras models
├── data/             # Test and example image data
├── app.py            # Main application script
├── requirements.txt  # Python dependencies
└── README.md         # Project documentation
```

---

## 🔬 Future Improvements

- 🛡️ **Expand Helmet Color Range**: Include more helmet color categories.
- 🖼️ **Higher Resolution Support**: Optimize for HD video streams.
- 📊 **Analytics Dashboard**: Integrate to track PPE compliance over time.
- 🌐 **Cloud Deployment**: Deploy the app on cloud platforms for scalability.

---

## 🤝 Contributing
Contributions are welcome! Feel free to submit a pull request or report an issue.

---

## 📜 License
This project is licensed under the MIT License. See the LICENSE file for details.

---

## ❤️ Acknowledgements
Special thanks to all open-source contributors and the deep learning community for resources and inspiration.

---

## 📧 Contact
For questions or support, reach out at your-email@example.com.

