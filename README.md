# Procurement RFx Timeline Predictor for Industrial Assets

## Objective

This project aims to streamline and automate the procurement process in industrial environments (e.g., refineries) by predicting the timeline of RFx (Request for [Quotation/Proposal/Information]) cycles. Using machine learning, the app forecasts the total duration in days based on key procurement features. A Streamlit-based interface enables interaction, and a Power BI dashboard (optional) offers strategic insights into delays and bottlenecks.

---

## Core Features

### App Interface (Streamlit)
- Lightweight frontend for user input and prediction results.
- Displays similar historical RFx cases for transparency and learning.

### Dashboard Layer (Power BI) *(Optional but Valuable)*
- Monitors patterns and bottlenecks:
  - Average procurement time by category
  - Vendor-wise delay analysis
  - Weekly/monthly timeline deviations
  - Departmental performance insights

### ML Model (In Progress)
- Predicts the total duration (in days) for completing an RFx cycle.
- Input features include:
  - **Material Category**: Chemicals, Heavy Equipment, Spare Parts, etc.
  - **Vendor Type**: Local, National, International
  - **Urgency Level**: Low, Medium, High
  - **Mode of Tender**: Open, Limited, Proprietary
  - **Estimated Cost**: Continuous numeric input
  - **Department**: Mechanical, Electrical, Instrumentation
  - **Historic Delays**: Yes/No (Boolean)
- **Target**: Procurement Completion Days

---

##  Tech Stack

| Component      | Tools Used                           |
|----------------|--------------------------------------|
| Language       | Python                               |
| Libraries      | `pandas`, `scikit-learn`, `xgboost`  |
| Interface      | Streamlit                            |
| Dashboard      | Power BI *(Optional)*                |
| Dataset        | Dummy CSV (~300–500 rows)            |

---

## Industry Relevance

- **Procurement Automation**: Mimics predictive automation in procurement cycles — aligns with industry demands.
- **Scalability**: Logic can be extended to real refinery datasets.
- **Decision Support**: BI layer helps procurement heads identify inefficiencies.

---

## 🚀 Getting Started

1. **Clone this repository**
   ```bash
   git clone https://github.com/your-username/procurement-rfx-predictor.git
   cd procurement-rfx-predictor
   ```
2. Install dependencies
3. ```bash
   pip install -r requirements.txt
   ```
 ---

 ## Project Structure
```bash
procurement-rfx-predictor/
│
├── data/
│   └── dummy_procurement_data.csv
│
├── model/
│   └── rf_model.pkl
│
├── app.py
├── requirements.txt
├── README.md
└── LICENSE
```

---
**License**
This project is licensed under the MIT License.

**Contribution**
I welcome contributions! Please open issues or submit pull requests for bug fixes, feature additions, or enhancements.

