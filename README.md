
# 🎥 Live Video Broadcaster

A **live video broadcasting web app** where you can apply real-time **background blur** or **custom background** to your webcam feed — and use it on platforms like **Google Meet**, **Zoom**, or **Twitch** with the help of a **virtual camera**.

---

## 🚀 Features

- 📸 Select and stream from any connected camera
- 🎚️ Adjust FPS (Frames Per Second)
- 🌫️ Control blur strength for background blur
- 🖼️ Switch between:
  - No background
  - Blur background
  - Custom image background
- 🔄 OBS and HD Camera support
- 🧠 Real-time person segmentation using **YOLOv8**

---

## 📷 Tech Stack

- **Python**
- **FastAPI** – for the backend API and serving the UI
- **OpenCV** – for video processing
- **Ultralytics YOLOv8** – for human segmentation
- **PyVirtualCam** – to create a virtual webcam
- **HTML/CSS/JavaScript** – for the frontend UI

---

## 🛠️ How to Run the Project

### 1. Clone the Repository
```bash
git clone https://github.com/rahulis-live/livevideoBroadcaster.git
cd livevideoBroadcaster
```

### 2. Install Dependencies
Make sure you have Python 3.10+ and [ffmpeg](https://ffmpeg.org/) installed.

```bash
pip install -r requirements.txt
```

Also, install `pyvirtualcam` dependencies (on Windows):
```bash
pip install pyvirtualcam
```

### 3. Download the YOLOv8 Model

Place your `yolov8m-seg.pt` model inside the project root.

> ⚠️ **Note**: The file is large (~52MB). GitHub might warn you about the size. You can use Git LFS or external hosting if needed.

### 4. Run the App
```bash
uvicorn main:app --reload
```

Then open your browser and go to:
```
http://localhost:8000
```

---

## 📺 Usage

1. Select your webcam from the dropdown.
2. Set FPS, blur strength, and background type.
3. Click **Start Stream**.
4. Open **Google Meet / Zoom / Twitch**, and choose **OBS Camera** or **Virtual Camera** as your webcam source.

---

## 🐞 Known Issues

- Large models like `yolov8m-seg.pt` may exceed GitHub's recommended file size.
- Ensure your webcam isn't already in use by another app.
- Virtual camera may require OBS or additional drivers on some systems.

---

## 📸 Screenshots / Demo (Optional)

> Add demo GIF or YouTube link here.

---

## 🤝 Contributing

Pull requests are welcome. Feel free to open issues for suggestions or bugs.

---

## 📜 License

MIT License

---

## 🙏 Credits

- [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)
- [PyVirtualCam](https://github.com/letmaik/pyvirtualcam)
- [FastAPI](https://fastapi.tiangolo.com/)

---

## 📬 Contact

For feedback or collaboration:
📧 rahulchandran.liv3@gmail.com  


