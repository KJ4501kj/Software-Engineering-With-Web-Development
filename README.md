# 🛳️ Titanic Survival Prediction Web App

This project is a containerized AI-powered web application that predicts whether a passenger would have survived the Titanic disaster. Users can tweak input parameters, test multiple ML models, and explore results interactively. 

---

## 🚀 About the Project

> “Get ready to embark on an exciting journey with our cutting-edge web application, driven by the power of artificial intelligence! Discover if you would have survived the legendary Titanic disaster as you explore and tweak various intriguing parameters. This isn’t just a web app—it’s your gateway to experiencing firsthand the capabilities of AI in a fun and engaging way!”  

---

## 📦 Repository Structure

Main Git repository:  
🔗 [`docker-compose`](https://mygit.th-deg.de/schober-teaching/student-projects/ain-23-software-engineering/ss-25/Sosyo/docker-compose.git)

Includes the following **submodules**:
- [`web-frontend`](https://mygit.th-deg.de/schober-teaching/student-projects/ain-23-software-engineering/ss-25/Sosyo/web-frontend.git)
- [`web-backend`](https://mygit.th-deg.de/schober-teaching/student-projects/ain-23-software-engineering/ss-25/Sosyo/web-backend.git)
- [`model-backend`](https://mygit.th-deg.de/schober-teaching/student-projects/ain-23-software-engineering/ss-25/Sosyo/model-backend.git)

---

## 🛠️ Setup Instructions

### 1. Clone the Repositories

Clone the main repo along with all submodules:

```bash
git clone --recurse-submodules https://mygit.th-deg.de/schober-teaching/student-projects/ain-23-software-engineering/ss-25/Sosyo/docker-compose.git
cd docker-compose
```

> If you forgot to use `--recurse-submodules`, you can initialize them later:
```bash
git submodule update --init --recursive
```

---

### 2. Start the Application

Build and run the app using Docker Compose:

```bash
docker-compose up -d --build
docker-compose up
```

Once started, visit the app at:  
📍 **http://localhost:8080**

---

## 🧪 Testing

### ✅ Web Frontend – Cypress E2E Tests

E2E Tests will automatically runs with Docker command, but if you want to run it separately then,

```bash
docker-compose run --rm cypress
```

---

### ✅ Web Backend – Pytest

```bash
docker-compose run --rm backend pytest
```

---

### ✅ Model Backend – Pytest

```bash
docker-compose run --rm model-trainer pytest
```

---

## 🔐 Admin Access

| Role  |        Email        |                          Password                            |
|-------|---------------------|--------------------------------------------------------------|
| Admin | sosyo2025@gmail.com | Register with "sosyo2025@gmail.com" and create your password |


---

## 💡 Features

- 🔍 Predict Titanic survival using 5 ML models:
  - Random Forest
  - Decision Tree
  - KNN
  - Support Vector Machines
  - Logistic Regression
- 👥 User registration and login
- 📊 Real-time prediction updates
- 🔁 Model selection (restricted by user type)
- 🧠 Admins can train/delete models
- 📜 History of last 10 predictions (for logged-in users)
- 🌐 SPA built in **React**
- 📦 Fully containerized with **Docker**
- 🌍 Routed via **Nginx reverse proxy**
- 🧪 Tests run on every commit via **GitLab CI**

---

## 👨‍👩‍👦 Team Members

| Name                          | Matriculation Number |
|-------------------------------|-----------------------|
| Jenil Kevadiya                | 22204227              |
| Krunal Ashvinbhai Koladiya    | 22306168              |
| Sarthik Ashokbhai Jagani      | 22306164              |
| Shubham Hareshbhai Mangaroliya| 22306211              |
| Divyam Kalpeshbhai Maniya     | 22306364              |

---

## 🧾 License

MIT License

---
