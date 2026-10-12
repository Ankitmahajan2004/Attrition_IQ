# AttritionIQ: HR Attrition Analysis

An end-to-end HR analytics project that explores employee attrition using **Snowflake**, **Python**, and **Streamlit**.

## 🚀 Live Demo

**[Open the live app](https://attritioniq-xppbl7w9cvmd4tpu3szqwp.streamlit.app/)**

> **Note:** The live demo needs no login. To run the project locally, you need your own Snowflake account.

## 📌 Overview

Employee attrition is costly for any company. This project loads HR data from Snowflake, analyses what drives employees to leave, and shows the results in an interactive dashboard.

## 🛠️ Tech Stack

- **Data warehouse:** Snowflake (SQL)
- **Analysis:** Python, pandas, NumPy
- **Visualization:** Matplotlib, Seaborn / Plotly
- **App:** Streamlit (deployed on Streamlit Community Cloud)

## 🔄 Data Pipeline

1. Raw HR data is loaded into Snowflake.
2. Data is cleaned using SQL (trimmed text, type casting, duplicates removed, missing values handled).
3. Python connects to Snowflake and reads the final table.
4. Analysis is done on attrition by department, role, age, salary, etc.
5. The Streamlit app displays the results.

## 📂 Project Structure

```
hr_attrition/
├── app.py                  # Streamlit dashboard
├── requirements.txt
├── .env.example            # Template for credentials
└── README.md
```

## ⚙️ Run Locally

**1. Clone the repo**
```bash
git clone https://github.com/Ankitmahajan2004/hr_attrition.git
cd hr_attrition
```

**2. Create a virtual environment and install packages**
```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

**3. Add your own Snowflake credentials**

Copy `.env.example` to `.env` and fill in your values:
```
SNOWFLAKE_USER=
SNOWFLAKE_PASSWORD=
SNOWFLAKE_ACCOUNT=
SNOWFLAKE_WAREHOUSE=
SNOWFLAKE_DATABASE=
SNOWFLAKE_SCHEMA=
```

**4. Run**
```bash
streamlit run app.py
```

## 🔐 Security

Credentials are never committed. `.env` is listed in `.gitignore`, and the deployed app reads its credentials from Streamlit Secrets.

## 👤 Author

**Ankit Mahajan**
GitHub: [@Ankitmahajan2004](https://github.com/Ankitmahajan2004)
