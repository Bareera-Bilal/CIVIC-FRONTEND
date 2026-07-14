# Civic- AI Powered Smart Civic Complaint Management System

> **Transforming civic issue reporting with Artificial Intelligence, automation, and real-time transparency.**

![FastAPI](https://img.shields.io/badge/FastAPI-Python-green)
![React](https://img.shields.io/badge/React-Frontend-61DAFB)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-green)

---

# Overview

**Civic AI** is an AI-powered civic complaint management platform that enables citizens to report public issues by simply uploading a photo. Instead of manually selecting departments or categories, Artificial Intelligence automatically detects the issue, estimates its severity, prevents duplicate complaints, assigns the responsible government department, and provides real-time tracking until resolution.

The platform improves transparency, reduces duplicate reports, speeds up complaint handling, and helps authorities prioritize issues using AI.

---

# Problem Statement

Citizens regularly face problems such as:

- Garbage accumulation
- Potholes
- Water leakage
- Broken street lights
- Fallen trees
- Road damage
- Damaged public property
- Illegal dumping

Current complaint systems suffer from:

- Manual categorization
- Duplicate complaints
- Slow response time
- Lack of transparency
- No intelligent prioritization
- Fake or irrelevant reports

These inefficiencies delay issue resolution and reduce citizen trust. :contentReference[oaicite:0]{index=0}

---

# Our Solution

CivicAI uses Artificial Intelligence to automate the complete complaint lifecycle.

The system:

- Detects the civic issue from an uploaded image
- Identifies severity level
- Detects duplicate complaints
- Automatically routes complaints to the correct department
- Generates AI descriptions
- Tracks complaint progress in real time
- Displays complaints on an interactive map
- Prioritizes complaints using AI

---

# Features

## AI Image Detection

Upload a photo and AI automatically identifies:

- Garbage
- Potholes
- Water Leakage
- Broken Street Lights
- Road Damage
- Drain Overflow

---

## AI Severity Prediction

Every complaint is classified into:

- Low
- Medium
- High
- Critical

---

## Duplicate Complaint Detection

Instead of creating multiple complaints for the same issue, CivicAI checks:

- Image similarity
- Nearby complaints
- GPS Location
- Complaint category

If already reported, users can support (upvote) the existing complaint.

---

## Automatic Department Routing

AI assigns complaints directly to departments like:

| Issue | Department |
|--------|------------|
| Garbage | Municipality |
| Road Damage | PWD |
| Street Light | Electricity Department |
| Water Leakage | Water Works |
| Fallen Trees | Forest Department |

---

## Interactive Complaint Map

Every complaint appears on a live map with color-coded status.

- 🟢 Solved
- 🟡 In Progress
- 🔴 Pending

---

## Smart Priority Score

Priority is calculated using:

- Severity
- Number of supporting citizens
- Nearby schools
- Nearby hospitals
- Traffic density
- Complaint age

---

## Live Complaint Tracking

Complaint lifecycle:

```
Submitted
      ↓
Received
      ↓
Assigned
      ↓
Officer Accepted
      ↓
Work Started
      ↓
Completed
```

---

## AI Description Generator

Instead of typing long descriptions, AI automatically generates complaint summaries.

Example:

> "Garbage accumulation near the roadside causing unhygienic conditions."

---

## Before & After Images

Authorities upload proof after resolving complaints.

Users can compare:

- Before
- After

---

## Analytics Dashboard

Dashboard includes:

- Total complaints
- Solved complaints
- Pending complaints
- Department performance
- Resolution time
- Complaint categories

---

## Voice Complaint

Users can report issues using voice input.

---

## Offline Complaint Draft

Complaints are stored locally during internet outages and automatically submitted when connectivity returns.

---

## Notification System

Users receive notifications when:

- Complaint accepted
- Officer assigned
- Work started
- Complaint completed

---

## Community Rewards

Citizens earn points for:

- Verified complaints
- Helpful confirmations
- Community participation

---

## Fake Complaint Detection

AI checks for:

- Random images
- Downloaded images
- Low-quality uploads
- Unrelated photos

---

# Tech Stack

## Frontend

- React.js
- Tailwind CSS
- Axios - Javascript library used to send Http requests from front to back
- Leaflet / Google Maps - display maps on web Applications

## Backend

- FastAPI - High performance python framework
- Python
- MongoDB
- Pydantic - Python library used for data validation and parsing - the movement of data between variables, functions, components, or screens within a software application. (CORE PART OF FAST API)

## AI
WSQ
- **YOLOv8 (You Only Look Once v8)** – Deep learning object detection model used to identify civic issues such as potholes, garbage, water leaks, and damaged infrastructure from uploaded images.
- **OpenCV** – Computer vision library used for image preprocessing, enhancement, and analysis before AI inference.
- **EasyOCR (Optional)** – Optical Character Recognition library used to extract text from images, such as street signs or location markers.
- **Image Embeddings** – Generate feature vectors from uploaded images to identify visually similar complaints and prevent duplicate reports.
- **Rule-Based Priority Engine** – Calculates complaint priority based on factors such as severity, location, number of citizen upvotes, nearby hospitals/schools, and complaint age to help authorities address critical issues first.


---

# System Workflow

```
Citizen

     │

Upload Complaint Image

     │

AI Detects Problem

     │

AI Predicts

• Category
• Severity
• Confidence

     │

Duplicate Detection

     │

Auto Department Routing

     │

Complaint Stored

     │

Live Public Tracking

     │

Complaint Resolved
```

---

# Project Structure

```
CIVIC-AI/

├── frontend/
│   ├── src/
│   │   ├── app/
│   │   ├── components/
│   │   ├── hooks/
│   │   ├── services/
│   │   └── utils/
│
├── backend/
│   ├── AI/
│   ├── Models/
│   ├── Routes/
│   ├── Utils/
│   ├── config.py
│   ├── main.py
│   └── requirements.txt
│
├── docs/
├── README.md
```

---

# Installation

## Clone Repository
git clone https://github.com/Bareera-Bilal/CIVIC-FRONTEND.git
git clone https://github.com/Bareera-Bilal/CIVIC-BACKEND.git


```

---

## Backend

cd backend

python -m venv venv

# Windows
venv\Scripts\activate

pip install -r requirements.txt

uvicorn main:app --reload
```

Backend runs on

http://localhost:8000
```

---

## Frontend

cd frontend

npm install

npm run dev

Frontend runs on

http://localhost:3000


# Future Enhancements

- AI Risk Prediction
- IoT Sensor Integration
- Smart Municipality Dashboard
- Mobile Application
- SMS Alerts
- Government Portal Integration
- Predictive Maintenance
- AI Chat Assistant
- Multi-language Support



# Impact

CivicAI aims to:

- Improve civic transparency
- Reduce duplicate complaints
- Speed up complaint resolution
- Increase citizen engagement
- Assist municipalities using AI-powered analytics
- Enable data-driven urban governance

---

# Developed By
TEAM: INFICODE


GitHub:
https://github.com/Bareera-Bilal

# If you like this project : Give this repository a ⭐ on GitHub and support the project.