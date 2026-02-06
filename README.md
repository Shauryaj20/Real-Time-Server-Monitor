# Real-Time-Server-Monitor
Full-stack dashboard monitoring CPU, RAM, and Disk metrics in real-time using Django &amp; React.
# Real-Time Server Resource Monitor 🖥️

![React](https://img.shields.io/badge/Frontend-React%20%7C%20Vite-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Django](https://img.shields.io/badge/Backend-Django%20REST-092E20?style=for-the-badge&logo=django&logoColor=white)
![TypeScript](https://img.shields.io/badge/Language-TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

## 📌 Project Overview
This is a **Full-Stack Single Page Application (SPA)** that monitors critical system metrics in real-time. Unlike static dashboards, this project bridges low-level OS data with a high-performance modern UI.

The system features a **Django REST API** that uses Python's `psutil` to inspect the host operating system, serving live telemetry to a **React + TypeScript** frontend every 3 seconds.

## 🚀 Key Features
* **Live Telemetry:** Polls backend every **3 seconds** for real-time CPU, RAM, and Disk usage.
* **Historical Tracking:** Visualizes the last **2 minutes** of system performance via dynamic line charts.
* **System Interface:** Uses Python's `psutil` library to interface directly with the OS kernel.
* **Advanced UI/UX:**
    * **Dark Mode Engine:** Built from scratch using **React Context API** and CSS Variables for seamless theme switching.
    * **Responsive Grid:** Modern 2-column layout designed with CSS Grid.

## 🛠️ Tech Stack
### Backend (Django)
* **Framework:** Django & Django REST Framework (DRF)
* **OS Interface:** `psutil` (Python Process and System Utilities)
* **API Pattern:** Stateless RESTful endpoints serving JSON data.

### Frontend (React)
* **Core:** React 18 (Vite) + TypeScript.
* **Visualization:** `Recharts` for high-performance doughnut and line charts.
* **State Management:** `useState` (Data Buffer), `useEffect` (Polling Interval), `useContext` (Theme State).

## 📸 Dashboard Preview
*(Upload your screenshot here)*

![Dashboard in Dark Mode](INSERT_LINK_HERE)
*Real-time CPU and Memory graphs in Dark Mode.*

## 🔧 Installation & Setup

### 1. Backend Setup (Django)
```bash
# Navigate to backend folder
cd my-django-api

# Install dependencies
pip install -r requirements.txt

# Run the API server (Runs at http://localhost:8000)
python manage.py runserver
pip install django djangorestframework django-cors-headers psutil

# Run the server
python manage.py runserver
