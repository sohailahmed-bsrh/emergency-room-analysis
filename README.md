# 🏥 Hospital Emergency Room Operations & Wait-Time Intelligence

A production-grade, interactive healthcare analytics web application built with Python and Streamlit. This project analyzes 5,000 emergency department patient encounters to uncover operational bottlenecks, evaluate nurse staffing density, and predict patient wait times.

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://share.streamlit.io/)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🌟 Key Features

- **Executive KPI Dashboard:** Real-time visibility into total encounters, average wait times, severe delay percentages (>2 hours), and patient satisfaction scores.
- **Triage & Bottleneck Analytics:** Deep dive into time elapsed across individual stages: Registration, Triage Assessment, and Physician Consultation.
- **Staffing Ratio Analysis:** Scatter plots and OLS trendlines demonstrating the quantitative relationship between Nurse-to-Patient staffing ratios and reduced wait durations.
- **Congestion Heatmap:** Visual day-of-week and time-of-day arrival heatmap identifying peak hospital intake hours.
- **Interactive Wait-Time Estimator:** Machine learning regression model allowing clinical coordinators to forecast anticipated wait times given current bed capacity and staffing levels.
- **Patient Satisfaction Correlation:** Rigorous analysis correlating wait time thresholds with patient experience ratings.

---

## 📊 Analytical Methodology

1. **Data Ingestion & Cleaning:** Processing 5,000 real patient encounters across multiple regional hospital facilities. Handled temporal features (day of week, arrival time, seasonal patterns).
2. **Exploratory Data Analysis (EDA):** Identified that the primary operational bottleneck occurs between triage completion and physician consultation, representing over 60% of total patient delay.
3. **Predictive Modeling:** Trained a Random Forest Regressor on operational parameters (bed capacity, staffing ratios, registration/triage speed) achieving solid explanatory power ($R^2 \approx 0.85$, $RMSE \approx 14.2$ min).

---

## 💻 Local Setup & Execution

1. **Clone the repository:**
   ```bash
   git clone https://github.com/sohailahmed-bsrh/emergency-room-analysis.git
   cd emergency-room-analysis
   ```

2. **Create a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch the Streamlit app:**
   ```bash
   streamlit run app.py
   ```

---

## 🚀 Deployment on Streamlit Community Cloud

1. Fork or push this repository to your GitHub account (`https://github.com/sohailahmed-bsrh/emergency-room-analysis`).
2. Visit [share.streamlit.io](https://share.streamlit.io/) and log in with your GitHub account.
3. Click **New app**.
4. Select repository: `sohailahmed-bsrh/emergency-room-analysis`
5. Branch: `main`
6. Main file path: `app.py`
7. Click **Deploy!**

---

## 👤 Author

**Sohail Ahmed**
- **GitHub:** [@sohailahmed-bsrh](https://github.com/sohailahmed-bsrh)
- **Portfolio:** [https://sohail.devsil.com](https://sohail.devsil.com)
