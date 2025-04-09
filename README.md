# **Face Recognition Attendance System**  

## **📌 Overview**  
A **desktop-based Face Recognition Attendance System** built with **Python, OpenCV (Haar Cascade), and PyQt5**. This application detects and recognizes faces in real-time, logs attendance, and provides a user-friendly interface for managing users, cameras, and subscriptions.  

### **✨ Key Features**  
✅ **Real-time Face Detection & Recognition**  
✅ **Attendance Logging (CSV)**  
✅ **User Management (Add/Delete Users)**  
✅ **Camera Management (IP/Webcam Support)**  
✅ **Unknown Face Capture & Logging**  
✅ **Admin Dashboard with UI/UX**  
✅ **Subscription & License Key Validation**  
✅ **Crash-Resistant & Optimized**  

---

## **🚀 Installation**  

### **Prerequisites**  
- **Python 3.8+**  
- **OpenCV (`pip install opencv-python`)**  
- **PyQt5 (`pip install PyQt5`)**  
- **Other Dependencies:**  
  ```bash
  pip install numpy pandas pillow opencv-contrib-python
  ```

### **Setup & Run**  
1. **Clone the Repository**  
   ```bash
   git clone https://github.com/your-repo/face-attendance-system.git
   cd face-attendance-system
   ```

2. **Run the Application**  
   ```bash
   python main.py
   ```

---

## **🛠️ Project Structure**  
```plaintext
face-attendance-system/
│
├── main.py                  # Entry point
├── config.json              # Stores camera & settings
│
├── database/                # SQLite database
│   ├── users.db             # User data
│   └── schema.sql           # DB schema
│
├── modules/                 # Core functionalities
│   ├── face_detection.py    # Haar Cascade detection
│   ├── user_management.py   # Add/Delete users
│   ├── camera_management.py # IP/Webcam handling
│   ├── video_processing.py  # Real-time video
│   ├── subscription.py      # License validation
│   └── alerts.py            # Error logging
│
├── ui/                      # PyQt5 UI
│   ├── main_window.py       # Dashboard
│   ├── login_window.py      # Admin login
│   ├── widgets.py           # Custom UI components
│   └── styles.css           # Styling
│
├── logs/                    # Logs (CSV + images)
├── unknown_faces/           # Captured unknown faces
└── Training_images/         # User training data
```

---

## **🎯 Usage**  

### **1. Login Screen**  
- **Default Admin Credentials**:  
  - Username: `admin`  
  - Password: `admin123`  

### **2. Dashboard**  
- **Live Camera Feed**: Displays real-time face detection.  
- **Left Panel**:  
  - **Add Known Person**: Upload or capture images.  
  - **Users**: View/Delete registered users.  
  - **License**: Validate subscription key.  
- **Right Panel**:  
  - **Logs**: Displays unknown faces and errors.  

### **3. Adding a User**  
1. Click **"Add Known Person"**.  
2. Choose:  
   - **Upload Images** (from PC)  
   - **Capture Images** (via webcam)  
3. Enter **user name** and save.  

### **4. Attendance Logging**  
- Detected faces are logged in `attendance.csv` with:  
  - **Date**  
  - **Name**  
  - **Camera Position**  
  - **In/Out Time**  

### **5. Handling Unknown Faces**  
- Unknown faces are saved in `unknown_faces/` with timestamps.  
- Admins can later **label and retrain** the model.  

---

## **🔒 Subscription & Licensing**  
- **License Key**: Required for premium features.  
- **Default Key**: `MY-VALID-KEY` (for testing).  
- **Admin Panel**:  
  - Add/Update license keys.  
  - Restrict features based on subscription.  

---

## **📝 Notes**  
- **Haar Cascade vs. DNN**:  
  - This app uses **Haar Cascade** (lightweight but less accurate).  
  - For better accuracy, consider **DNN-based models** (e.g., `face_recognition` library).  
- **Performance**: Optimized for **low-end PCs**.  
- **Extensibility**: Built with **Factory Design Pattern** for modularity.  

---

## **📜 License**  
MIT License © 2023  

---

## **📧 Contact**  
For issues/feedback:  
📩 **shaikhmustakim2942@gmail.com.com**  
🌐 **[https://github.com/your-repo](https://github.com/MUSTAKIMSHAIKH2942/MUSTAKIMSHAIKH2942/blob/main/README.md)**  

---

### **🎉 Ready to Use!**  
Run `python main.py` and start tracking attendance with AI! 🚀
