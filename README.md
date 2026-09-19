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

Running Locally
1. Clone the repository
git clone <repository-url>
cd Leukemia_survival-prognosis
2. Install dependencies
pip install -r requirements.txt
3. Run the application
python app.py
