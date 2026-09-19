# Leukemia Survival Prognosis

A web-based leukemia survival prognosis application that uses trained survival models to estimate patient survival outcomes from clinical data.

## Overview

This project provides an interactive dashboard for leukemia survival analysis and prognosis.

The application:
- Accepts patient clinical information as input
- Processes and transforms the input using the trained preprocessing pipeline
- Generates survival predictions using trained survival models
- Displays predicted survival information through an interactive web interface
- Supports cohort-level analysis and treatment simulation

## Features

- Patient-specific survival prognosis
- Interactive clinical data input
- Survival analysis using trained DeepHit and Log-Hazard models
- Automated preprocessing and feature selection
- Cohort analysis and visualization
- Treatment simulation
- Docker-based deployment support

## Tech Stack

- **Backend:** Python, Flask
- **Frontend:** HTML, CSS, JavaScript
- **Models:** DeepHit, Log-Hazard
- **Data Processing:** Scikit-learn, NumPy, Pandas
- **Deployment:** Docker

## Project Structure

```text
leukemia-prognosis-app/
├── app.py
├── inference_engine.py
├── index.html
├── script.js
├── style.css
├── requirements.txt
├── Dockerfile
├── Procfile
├── models/
│   ├── deephit_final_leukemia_best.pth
│   ├── loghazard_final.pth
│   ├── feature_selector_k60.pkl
│   ├── imputer.pkl
│   ├── label_trans_40.pkl
│   ├── labtrans_50.pkl
│   └── scaler.pkl
└── README.md
```

## How It Works
Patient Clinical Data
        ↓
Input Validation
        ↓
Data Preprocessing
        ↓
Feature Selection
        ↓
Trained Survival Models
        ↓
Survival Prediction
        ↓
Interactive Dashboard  


## Running Locally
1. Clone the Repository
git clone https://github.com/Sanjaytalluri112/Leukemia_survival-prognosis.git
cd Leukemia_survival-prognosis

2. Create a Virtual Environment
macOS / Linux
python3 -m venv venv
source venv/bin/activate

Windows
python -m venv venv
venv\Scripts\activate

3. Install Dependencies
pip install -r requirements.txt

5. Run the Application
python app.py

Docker

The project includes a Dockerfile for containerized deployment.

1. Build the Docker Image
docker build -t leukemia-prognosis .

2. Run the Container
docker run -p 5000:5000 leukemia-prognosis
