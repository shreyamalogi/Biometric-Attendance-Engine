

# 📸 Biometric Attendance Engine: Real-Time Identity Verification

**🏆 Award-Winning Innovation: Selected as a Finalist among 100+ competing teams (Team Mavericks)**

## 📖 The "Problem-to-Solution" Narrative

Manual attendance tracking is a high-friction administrative task prone to data latency and "proxy" errors. As a core developer for **Team Mavericks**, I collaborated on building an AI-powered ecosystem designed to make identity verification seamless and totally automated.

Our mission was to move facial recognition out of a static script and into a functional, secure web application capable of handling diverse input streams in real-time.

---

## 🏗️ System Architecture: Three-Mode Versatility

To ensure the system was practical for real-world institutional environments, we engineered **3 specialized processing modes**:

* 
**Live Feed**: Real-time identification via active webcam streams for immediate classroom logging.


* 
**Static Image**: Batch-processing of photographs for post-event verification and archival.


* 
**Video Playback**: Asynchronous analysis of recorded footage to register attendance from pre-captured video files.



---

## 🛠️ The Technical Stack

**Core Developer & Backend Integration: Shreya Malogi** 

I contributed to the full-cycle development of this project, with primary ownership of the **Backend Architecture** and **Data Integration Layer**:

### **AI & Computer Vision**

* **Methodology**: Utilized **HOG (Histogram of Oriented Gradients)** for robust facial feature encoding, ensuring the model identifies structural shapes rather than simple pixel intensity.
* **Libraries**: Implemented **OpenCV** and **Dlib** for the 68-point landmark detection required for biometric precision.
* **Identity Logic**: Integrated `face_recognition` libraries to map detected landmarks against a trained encoding database.

### **Backend & Systems Engineering**

* **Framework**: Built the core application logic using **Flask** to manage multi-part real-time video streaming.
* **Database (ORM)**: Engineered a relational schema using **SQLAlchemy** to manage `Users`, `Students`, and `Semesters`.
* **Persistence**: Leveraged **SQLite** for structured data storage of all attendance logs and user credentials.
* **Security**: Integrated **Werkzeug** for secure password hashing and **Flask-Login** for protected administrative sessions.

### **Data & UI Layer**

* **Reporting**: Utilized **Pandas** to automate the transformation of raw biometric signals into structured CSV attendance reports.
* **Frontend**: Designed a responsive interface using **HTML, CSS, Bootstrap**, and **Jinja2** templating for dynamic data rendering.

---

## 🤯 Engineering Challenges & Optimization

* **Latency Mitigation**: We encountered significant processing lag when integrating external IP cameras. We optimized the frame-buffer cycle to maintain real-time performance.
* 
**State Management**: Orchestrating the logic to switch between live, static, and video inputs without memory leaks required a modular system architecture.



---

## 🚀 Impact & Recognition

By focusing on a user-centric design—creating an interface for both Admins and Teachers—our project was selected as a **Finalist among 100+ teams**. This project proves my ability to collaborate in a high-pressure environment to deliver a secure, scalable AI product.

---

### 📥 Setup & Technical Deployment

1. **Clone & Install**: `pip install -r requirements.txt`
2. **Database**: The system initializes `DataBase.db` on launch using the SQLAlchemy models.
3. **Run**: Execute `python main.py` and access the dashboard at `localhost:5000`.

---

**Would you like me to find some relevant Berlin-based job postings that specifically look for Flask and OpenCV skills to help you start applying?**
