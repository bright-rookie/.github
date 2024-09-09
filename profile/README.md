# AI-SAFE: Child Abuse Detection for Medical Professionals

**AI-SAFE** is a project designed to assist medical professionals in identifying potential child abuse cases using AI-driven analytics. The system aims to enhance early detection and help overcome the current challenges medical staff face when assessing child abuse, especially in high-pressure and time-limited environments.

## Overview

AI-SAFE leverages both **front-end** and **back-end** systems to analyze medical data and provide predictive insights. The project is focused on aiding doctors, especially in emergency and pediatric care, in accurately reporting and managing cases where child abuse might be suspected.

### Key Features:
- **Medical Data Processing:** Use of AI to analyze patient data (e.g., medical records, X-rays, patient history).
- **Predictive Analytics:** AI models to calculate child abuse risk based on historical and real-time data.
- **Doctor Assistance:** Tools for doctors to report or escalate cases based on AI outputs.

## Frontend (Streamlit)
The frontend interface is built using **Streamlit** for ease of use by medical professionals. It allows them to:
- Input patient data, such as symptoms and medical history.
- Review AI-generated reports on child abuse risk.
- Generate reports to assist in documenting and escalating cases.

### Features:
- **Data Input:** Streamlit forms for inputting patient data.
- **Real-Time Feedback:** AI-generated risk analysis based on input data.
- **Reporting:** Downloadable reports for documentation and case escalation.

### Getting Started with Frontend:
1. Clone the repository:
   ```bash
   git clone https://github.com/your-org/ai-safe.git
   cd ai-safe/frontend
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the app:
   ```bash
   streamlit run app.py
   ```

## Backend
The backend is responsible for processing medical data and applying the AI models. The backend handles tasks such as:
- **Data Processing:** Parsing electronic medical records (EMR) and imaging data.
- **AI Model Integration:** Running models to predict abuse risk based on various factors (e.g., patient demographics, medical history, X-ray results).
- **API:** A RESTful API for frontend-backend communication.

### Getting Started with Backend:
1. Navigate to the backend folder:
   ```bash
   cd ai-safe/backend
   ```
2. Set up a Python virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```
3. Run the API server:
   ```bash
   uvicorn app:app --reload
   ```

## How It Works

1. **Data Input:** Medical professionals enter patient data into the Streamlit interface (e.g., symptoms, lab results, and medical history).
2. **AI Analysis:** The backend processes the data using pre-trained models to assess risk factors for child abuse.
3. **Decision Support:** AI-SAFE provides risk scores and generates reports to help doctors make informed decisions on reporting or escalating cases.
