# Leukemia Survival Prognosis

A web-based leukemia survival prognosis application that uses trained survival models to estimate patient survival outcomes from clinical data.

## Overview

This project provides an interactive dashboard for leukemia survival analysis and prognosis.

The application:

- Accepts patient clinical information as input
- Processes and transforms the input using trained preprocessing components
- Generates survival predictions using trained survival models
- Displays prediction results through an interactive web interface
- Supports cohort-level analysis and treatment simulation

## Features

- Patient-specific survival prognosis
- Interactive clinical data input
- DeepHit and Log-Hazard survival models
- Automated preprocessing and feature selection
- Cohort-level analysis and visualization
- Treatment simulation
- Docker-based deployment support

## Tech Stack

| Component | Technology |
|---|---|
| Backend | Python, Flask |
| Frontend | HTML, CSS, JavaScript |
| Survival Models | DeepHit, Log-Hazard |
| Data Processing | NumPy, Pandas, Scikit-learn |
| Deployment | Docker |

## Project Structure

```text
Leukemia_survival-prognosis/
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

The application follows the pipeline below:

```text
Patient Clinical Data
        │
        ▼
Input Validation
        │
        ▼
Data Preprocessing
        │
        ▼
Feature Selection
        │
        ▼
Trained Survival Models
        │
        ▼
Survival Prediction
        │
        ▼
Interactive Dashboard
```

## Running Locally

### 1. Clone the Repository

```bash
git clone https://github.com/Sanjaytalluri112/Leukemia_survival-prognosis.git
cd Leukemia_survival-prognosis
```

### 2. Create a Virtual Environment

#### macOS / Linux

```bash
python3 -m venv venv
source venv/bin/activate
```

#### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
python app.py
```

The Flask application will start locally.

Open the application in your browser:

```text
http://127.0.0.1:5000
```

### 5. Stop the Application

Press:

```text
Ctrl + C
```
