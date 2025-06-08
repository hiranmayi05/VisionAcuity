# Automated Vision Clarity Measurement Using AI

An AI-powered vision test system that enables users—especially athletes—to assess their visual acuity independently and accurately using face detection, distance calibration, and dynamically generated Landolt C charts.

*Automated Vision Clarity Measurement** is an AI-driven system that lets users assess their eyesight just by sitting in front of a webcam. No need for printed charts or professional supervision.

---

## 📌 Project Overview

This project addresses the challenge of making vision testing accessible, standardized, and self-administered. Traditional vision tests require human supervision and fixed setups. Our tool uses computer vision and AI to:
- Detect the user's face and measure their distance from the screen
- Generate precise Landolt C optotypes scaled correctly to distance and screen size
- Adaptively test visual acuity based on user responses
- Deliver results in standard formats like 6/6, 6/9, etc.

---

## 🧠 Key Features

- **Face Detection with YuNet**  
  Real-time, lightweight face detection using YuNet model. Enables accurate facial tracking and distance estimation.

- **Focal Length Calibration**  
  Uses user's face width and known one-arm distance to calculate webcam focal length for distance estimation.

- **Screen Calibration via Credit Card**  
  Allows accurate symbol sizing by matching a digital rectangle to a real credit card, accounting for pixel density.

- **Landolt C Chart Generation**  
  Programmatic drawing of Landolt C optotypes using HTML5 Canvas with dynamic orientation and size control.

- **Adaptive Vision Testing**  
  Test difficulty adjusts automatically based on user responses. Smaller C = better acuity.

- **Result Interpretation**  
  Vision scores are calculated in standardized formats like 6/6, 6/12, etc., based on the smallest correctly identified C.

---

## 🛠️ Technologies Used

- **Frontend:** HTML5, CSS3, JavaScript
- **Canvas Rendering:** HTML5 Canvas API
- **Face Detection Model:** [YuNet](https://arxiv.org/abs/2301.07055) (Tiny CNN-based face detector)
- **AI Calibration Logic:** JavaScript-based focal length and screen size estimators

---

## 🚀 How It Works

1. **User positions themselves at arm’s length from the webcam.**
2. **YuNet detects the face and estimates face width in pixels.**
3. **System calibrates camera focal length.**
4. **User matches a rectangle to a credit card to calculate screen PPI.**
5. **Landolt C symbols are drawn on screen, dynamically sized and rotated.**
6. **User responds using keyboard or mouse (future: voice input).**
7. **System evaluates response and adjusts difficulty.**
8. **Final result is presented in standard vision format.**

---

## Test Results & Accuracy

- Achieves consistent acuity scoring similar to traditional Snellen/optometric tests.
- Validated for working in varying lighting conditions with high accuracy via YuNet.
- All screen calibration and distance estimation handled without external tools.

---

## 👨‍💻 Contributors

- **P. Koushik** – [S20220010156]
- **N. Anuroop Reddy** – [S20220010147]
- **M. Hiranmayi** – [S20220010146]  
  
---

## 📄 License

This project is for academic and research purposes only. For further use, contact the project guide or contributors.

---

## 📬 Contact

If you're interested in this project or want to collaborate, feel free to connect!

Mail : hiranmayi2005@gmail.com

Github : https://github.com/hiranmayi05
