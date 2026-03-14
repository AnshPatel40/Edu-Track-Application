# 🎓 EduTrack – Student Academic Data Analytics & Performance Insights System

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-Framework-FF4B4B.svg)](https://streamlit.io/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-Database-336791.svg)](https://www.postgresql.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> A modern academic analytics platform designed to transform raw student datasets into meaningful, actionable insights.

EduTrack enables educational institutions—schools, colleges, and training centers—to upload academic data and automatically generate performance analytics, visual dashboards, and downloadable reports. Built on a modular SaaS architecture using industry-standard Python data analytics technologies, it supports scalable deployment across multiple organizations simultaneously.

---

## 📖 Table of Contents
- [Features](#-features)
- [System Architecture](#-system-architecture)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [Contributing](#-contributing)

---

## ✨ Features

EduTrack aims to simplify academic monitoring and enable data-driven decision-making for improving student outcomes through a robust feature set:

* **Multi-Institution Tenancy:** Secure login system supporting multiple institutions on a single deployment.
* **Role-Based Access Control (RBAC):** Customized dashboards and permissions for Admins and Teachers.
* **Automated Data Pipeline:** Seamless dataset uploads (CSV/Excel) coupled with automated data cleaning and preprocessing.
* **Advanced Analytics:** In-depth correlation analysis between attendance and marks, alongside automated identification of top performers and at-risk students.
* **Interactive Visualization:** Dynamic, responsive charts and interactive analytics dashboards.
* **Export & Reporting:** Export cleaned datasets and comprehensive analytics reports in CSV or PDF formats.
* **Responsive UI:** Fully responsive design optimized for desktop, tablet, and mobile viewing.

---
---

## 🧠 Tech Stack

EduTrack leverages a robust and modern technology stack to deliver a seamless analytics experience:

| Component | Technology |
| :--- | :--- |
| **Programming Language** | Python |
| **Data Analytics** | pandas, NumPy |
| **Visualization Tools** | Plotly, Seaborn, Matplotlib |
| **Dashboard Framework** | Streamlit |
| **Database** | PostgreSQL |
| **Security & Auth** | bcrypt |

---

## 🏗️ System Architecture

EduTrack follows a modular, three-layer architectural pattern ensuring separation of concerns, security, and scalability:

1. **Client Layer:** User devices (web browsers or mobile devices)
2. **Application Layer:** Python backend services handling authentication, data processing, and analytics
3. **Data Layer:** Cloud database storing institutions, users, datasets, and analytics results

- EduTrack utilizes a secure and scalable multi-tier architecture, ensuring separation of concerns and data integrity. The system flow, from user interaction to data storage and reporting, is visualized in the diagram below:

<br>
<div align="center">
  ![alt="EduTrack System Architecture Diagram"]
</div>
<br>

**Key Architectural Flows:**

1.  **Client Layer:** Users interact via the **Web Dashboard Interface** (a Streamlit UI) across various devices.
2.  **Application Layer:** Handles authentication and all backend Python services.
3.  **Data Layer:** PostgreSQL stores institutional data, user profiles, datasets, and generated insights.
4.  **Reporting:** Data is exported as CSV/PDF from the Export System.

---
## 🚀 Getting Started

# Prerequisites
- Python 3.8 or higher
- PostgreSQL installed and running locally or via cloud
- Git

# Installation
1. Clone the repository
   - git clone [https://github.com/AnshPatel40/EduTrack.git](https://github.com/AnshPatel40/EduTrack.git)
     cd EduTrack
2. Create and activate a virtual environment
   - python -m venv venv
   # On Windows:
      venv\Scripts\activate
    # On macOS/Linux:
      source venv/bin/activate
   
3. Install dependencies
   - pip install -r requirements.txt
4. Environment Setup
   - DB_HOST=localhost
     DB_PORT=5432
     DB_USER=postgres
     DB_PASS=yourpassword
     DB_NAME=edutrack
     SECRET_KEY=your_secure_key
5. Run the Application
   - python -m streamlit run main_app.py
