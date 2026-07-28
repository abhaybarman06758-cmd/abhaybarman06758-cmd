# Face Recognition-Based Person Identification System

<div align="center">

# Face Recognition-Based Person Identification System

An AI-powered web application that identifies a person by matching an uploaded face image against a database of registered individuals and displays their stored information when a successful match is found.

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Node.js](https://img.shields.io/badge/Node.js-20+-339933?logo=node.js)
![React](https://img.shields.io/badge/React-19-61DAFB?logo=react)
![Express](https://img.shields.io/badge/Express.js-Backend-black?logo=express)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-47A248?logo=mongodb)
![Python](https://img.shields.io/badge/Python-Face_Recognition-3776AB?logo=python)

</div>

---

## Table of Contents

- **Overview**
- **Features**
- **System Workflow**
- **Tech Stack**
- **Project Structure**
- **Face Recognition Process**
- **Person Information**
- **Admin Features**
- **User Features**
- **Security Features**
- **Future Improvements**
- **Installation**
- **API Endpoints**
- **Screenshots**
- **Contributing**
- **License**
- **Author**

---

## Overview

The Face Recognition-Based Person Identification System is an AI-powered application that uses computer vision and face recognition techniques to identify individuals from an uploaded image.

The system stores a database of registered people's facial images and personal information. When a user uploads a new image, the application detects the face, extracts facial features, and compares them against all registered faces in the database.

If a matching face is found, the application retrieves and displays the corresponding person's details. Otherwise, it informs the user that no matching record exists.

This project can be used in educational institutions, offices, security systems, visitor management, and authorized identity verification applications.

---

## Features

-  Face Detection
-  AI-Based Face Recognition
-  Image Upload
-  Registered Person Database
-  Fast Face Matching
-  Display Person Details
-  No-Match Detection
-  Secure Authentication
-  Responsive User Interface
-  Admin Dashboard
-  Manage Registered Faces
-  Modern UI

---

## System Architecture

![Architecture](./docs/images/architecture.png)




## System Workflow

```text
              Upload Image
                    │
                    ▼
          Face Detection (AI)
                    │
                    ▼
      Extract Facial Embeddings
                    │
                    ▼
     Compare with Database Faces
                    │
        ┌───────────┴───────────┐
        │                       │
        ▼                       ▼
   Match Found             No Match
        │                       │
        ▼                       ▼
 Display Person Info      Show "No Match Found"
```

---

## Tech Stack

### Frontend

- React.js
- Tailwind CSS
- Axios
- React Router

### Backend

- Node.js
- Express.js
- JWT Authentication
- Multer

### AI / Computer Vision

- Python
- OpenCV
- face_recognition Library
- NumPy

### Database

- MongoDB
- Mongoose

### Other Tools

- Git
- GitHub
- Postman
- VS Code

---

## Project Structure

```bash
Face-Recognition-System/
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── controllers/
│   ├── routes/
│   ├── middleware/
│   ├── models/
│   ├── uploads/
│   ├── config/
│   └── server.js
│
├── ai/
│   ├── recognize.py
│   ├── encode_faces.py
│   └── dataset/
│
├── database/
│
├── README.md
│
└── package.json
```

---

## Face Recognition Process

1. Register people by uploading their images.
2. Generate facial embeddings.
3. Store embeddings in the database.
4. Upload a new image.
5. Detect the face.
6. Compare it with stored embeddings.
7. Return the matched person's information.

---

## Person Information

When a face is successfully recognized, the system can display:

- Full Name
- Unique ID
- Email
- Phone Number
- Department
- Designation
- Address
- Gender
- Date of Birth
- Profile Photo
- Registration Date

---

## Admin Features

- Login Authentication
- Register New Person
- Upload Multiple Images
- Edit Person Information
- Delete Records
- Search Person
- View Registered Database
- Export Data
- Manage Users
- Dashboard Analytics

---

## User Features

- Upload Image
- View Recognition Result
- Person Information
- Match Confidence Score
- Recognition History

---

## Security Features

- JWT Authentication
- Password Hashing
- Protected APIs
- Input Validation
- File Type Validation
- Secure Image Upload
- Role-Based Access Control
- Environment Variables

---

## Future Improvements

- Real-Time Camera Recognition
- Live CCTV Integration
- Multi-Face Detection
- Attendance System
- Mobile Application
- Cloud Storage
- Email Notifications
- SMS Alerts
- Face Mask Detection
- Anti-Spoofing Detection
- Liveness Detection

---

## Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/Face-Recognition-System.git
```

### Frontend

```bash
cd frontend
npm install
npm run dev
```

### Backend

```bash
cd backend
npm install
npm start
```

### AI Module

```bash
cd ai

pip install -r requirements.txt

python encode_faces.py

python recognize.py
```

---

## API Endpoints

### Authentication

```text
POST /api/auth/login
POST /api/auth/register
```

### Person

```text
POST   /api/person
GET    /api/person
GET    /api/person/:id
PUT    /api/person/:id
DELETE /api/person/:id
```

### Recognition

```text
POST /api/recognize
```

---

## Screenshots

```text
Login Page
Dashboard
Register Person
Upload Image
Recognition Result
Person Details
History
```

---

## Future AI Improvements

- Face Embedding Optimization
- DeepFace Integration
- YOLO Face Detection
- TensorFlow Models
- GPU Acceleration
- Faster Recognition
- Better Accuracy
- Cloud Deployment

---

## Contributing

Contributions are welcome.

1. Fork the repository.
2. Create your feature branch.
3. Commit your changes.
4. Push your branch.
5. Open a pull request.

---

## License

This project is licensed under the MIT License.

---

## Author

**Abhay Barman**

- GitHub: [https://github.com/ABHAYBARMAN067](https://github.com/ABHAYBARMAN067)
- LinkedIn: [https://linkedin.com/in/abhay-barman-9a0b3a277](https://linkedin.com/in/abhay-barman-9a0b3a277)

---

<div align="center">

### ⭐ If you like this project, please consider starring the repository.

Made with  using AI, Computer Vision, React, Node.js, Python, and MongoDB.

</div>
