## Solar Challenge Week 1 - Tenx Platform

This repository contains the work for **Week 0** of the **Tenx Platform Solar Data Discovery Challenge**.
The challenge focuses on solar data analysis for Benin, Sierra Leone, and Togo to support decision-making at **MoonLight Energy Solutions**.

---

## Project Objectives

- Profile and clean solar radiation datasets
- Perform EDA for each country
- Compare countries to find the best region for solar investment
- Build and deploy a dashboard using Streamlit

---

## How to Reproduce the Environment

To run this project on your local machine, follow these steps:

```bash
# 1. Clone the GitHub repository
git clone https://github.com/<your-username>/solar-challenge-week1.git
cd solar-challenge-week1

# 2. Create and activate a Python virtual environment
python -m venv venv             # On Windows: python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate

# 3. Install all dependencies
pip install -r requirements.txt

# 4. (Optional) Run GitHub Actions workflow (to test CI)
# This runs automatically on GitHub, but you can test locally using act or a similar tool
```

Make sure to use **Python 3.10+**.

---

## Folder Structure

```
├── .vscode/
│   └── settings.json
├── .github/
│   └── workflows/
│       └── ci.yml
├── .gitignore
├── requirements.txt
├── README.md
├── notebooks/
│   ├── benin_eda.ipynb
│   ├── togo_eda.ipynb
│   └── sierra_leone_eda.ipynb
├── scripts/
│   └── data_cleaning.py
├── data/
│   └── benin_clean.csv (ignored)
├── tests/
│   └── test_cleaning.py
└── app/
    ├── main.py
    ├── utils.py
```

---

## GitHub Branches

- `main`: Main branch
- `setup-task`: Environment & CI setup
- `eda-benin`, `eda-togo`, `eda-sierra-leone`: EDA for each country
- `compare-countries`: Country comparison notebook
- `dashboard-dev`: Streamlit dashboard code

---

## Deployment (Optional)

The dashboard will be deployed to [Streamlit Community Cloud](https://streamlit.io/cloud).
More details can be found in `app/README.md`.

---

## License

MIT License