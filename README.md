# 🎓 Face Recognition Attendance System

A Python-based Face Recognition Attendance System that automatically detects and recognizes registered faces using a webcam and records attendance in a CSV file. The project also includes a Flask web interface for real-time attendance monitoring.

## 🚀 Features

* 🔍 Real-time face detection and recognition
* 📷 Webcam-based attendance marking
* 👤 Recognizes registered users from stored face images
* 📅 Automatically records:

  * Name
  * Date
  * Time
  * Attendance Status (Present/Absent)
* 🌐 Flask-based web interface
* 📊 Attendance stored in CSV format
* ⚡ Fast and lightweight implementation using OpenCV and Face Recognition

## 🛠️ Technologies Used

* Python 3.x
* OpenCV
* Face Recognition (dlib)
* NumPy
* Pandas
* Flask

## 📂 Project Structure

```text
attendance/
│
├── app.py                  # Standalone attendance application
├── web.py                  # Flask web application
├── templates/
│   └── index.html          # Web interface
├── known_faces/            # Store registered face images
├── attendance.csv          # Attendance records
├── webattendance.csv       # Web attendance records
└── README.md
```

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/attendance.git
cd attendance
```

### 2. Create a virtual environment (Optional)

```bash
python -m venv venv
```

Activate it:

**Windows**

```bash
venv\Scripts\activate
```

**Linux / macOS**

```bash
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install opencv-python
pip install face_recognition
pip install flask
pip install pandas
pip install numpy
```

Or install all at once:

```bash
pip install opencv-python face_recognition flask pandas numpy
```

## 📸 Register Faces

Create a folder named:

```text
known_faces/
```

Place images of registered users inside the folder.

Example:

```text
known_faces/
│
├── Arjun.jpg
├── Rahul.jpg
├── Anjali.png
```

The filename will be used as the person's name during attendance.

## ▶️ Running the Project

### Option 1: Desktop Version

```bash
python app.py
```

### Option 2: Flask Web Version

```bash
python web.py
```

Open your browser and visit:

```
http://127.0.0.1:5000/
```

## 📄 Attendance Output

Attendance is saved in CSV format.

Example:

| Name  | Date       | Time     | Status  |
| ----- | ---------- | -------- | ------- |
| Arjun | 2026-07-05 | 09:12:45 | Present |
| Rahul | 2026-07-05 | 09:14:18 | Present |

## 📷 How It Works

1. Loads all registered face images.
2. Computes facial encodings.
3. Opens the webcam.
4. Detects faces in each frame.
5. Compares detected faces with registered faces.
6. Identifies matching individuals.
7. Records attendance with timestamp.
8. Saves attendance in a CSV file.

## 📌 Future Improvements

* Database integration (MySQL/PostgreSQL)
* User authentication
* Admin dashboard
* Attendance analytics and reports
* Email notifications
* QR code support
* Cloud deployment
* Mobile application

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a new branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

## 📜 License

This project is intended for educational and learning purposes. Feel free to modify and extend it according to your requirements.

## 👨‍💻 Author

**Arjun Shajan**

B.Tech Artificial Intelligence & Data Science

If you found this project useful, consider giving it a ⭐ on GitHub.
