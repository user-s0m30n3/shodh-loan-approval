# 📘 Policy Optimization for Financial Decision-Making  
### *Shodh Hiring – ML/AI Assessment*  

This repository contains my complete solution for the **Shodh Hiring ML/AI Assessment**, focused on optimizing loan-approval decisions using **Supervised Learning** and **Offline Reinforcement Learning**.

The project uses the **LendingClub Loan Dataset (2007–2018)** and follows all four tasks outlined in the official assignment PDF.

---

# 📂 Repository Structure

```
/project-root
│
├── notebook.ipynb              # Full workflow: EDA → Preprocessing → DL → RL
├── final_Report.pdf            # 2–3 page Shodh report
├── requirements.txt            # Python dependencies
└── README.md                   
```

---

# 🚀 Setup Instructions

## 1. Clone the Repository
```bash
git clone <your-repo-url>
cd <project-folder>
```

## 2. Create a Virtual Environment
```bash
python -m venv venv
source venv/bin/activate        # Linux / Mac
venv\Scripts\activate           # Windows
```

## 3. Install Dependencies
```bash
pip install -r requirements.txt
```

## 4. Download the Dataset

Download from Kaggle:  
**LendingClub Loan Data → accepted_2007_to_2018.csv**

Place the file in:

```
data/raw/accepted_2007_to_2018.csv
```

(Or update the path inside the notebook.)

---

# 📓 Notebook Contents

The single notebook (`notebook.ipynb`) contains the entire workflow:

### ✅ 1. Exploratory Data Analysis (EDA)
- Distribution plots  
- Loan status breakdown  
- Interest-rate boxplots  
- Missing value heatmaps  
- Summary statistics  
- Default share analysis  

### ✅ 2. Preprocessing & Feature Engineering
- Removal of leakage-heavy fields  
- Parsing percentage fields  
- One-hot encoding  
- Date parsing and credit history age  
- Missing value handling  
- Final feature selection  

### ✅ 3. Supervised Deep Learning Model
- Binary target creation  
- MLP classifier (TensorFlow/PyTorch)  
- Metrics: **AUC, F1-score**  
- Calibration curve  
- Threshold tuning for maximum economic value (EPV)  

### ✅ 4. Offline Reinforcement Learning (CQL)
- Single-step MDP environment  
- State, Action, Reward design  
- Synthetic action generation (deny actions)  
- CQL model via **d3rlpy**  
- Policy evaluation (Estimated Policy Value)  
- ML vs RL decision divergence analysis  

---

# 📊 Outputs Generated in the Notebook

- Interest rate distribution by loan status  
- Calibration curve (Predicted vs Actual Default Rate)  
- AUC & F1 metrics for logistic and MLP  
- RL policy EPV (negative, high-loss)  
- ML policy EPV (positive, profitable at threshold 0.09)  
- 17,196 ML–RL disagreements printed and analyzed  

---

# 📄 Final Report

The complete analysis is provided in:

```
Final_Report.pdf
```

It includes:
- EDA summary  
- Deep Learning model details  
- RL agent setup  
- Evaluation metrics  
- Profitability comparison (EPV)  
- Insights, limitations, and future improvements  

This PDF is the official submission for the Shodh assignment.

---

# ⚙️ Requirements

All dependencies are listed in:

```
requirements.txt
```

Typical libraries:

```
numpy
pandas
matplotlib
scikit-learn
tensorflow / torch
d3rlpy
tqdm
seaborn
```

Install them with:

```bash
pip install -r requirements.txt
```

---

# 🧪 Reproducibility

To reproduce the results:

1. Install dependencies  
2. Download & place the dataset  
3. Run all cells in `notebook.ipynb`  

All figures, metrics, RL policies, and tables will be generated automatically.

---

# 🙌 Contact

**Your Name**  
Email: sujay8208@gmail.com  


---

# 🎯 Ready for Submission

This repository includes:

- ✔ Notebook (EDA → DL → RL)  
- ✔ Final Report PDF  
- ✔ requirements.txt  
- ✔ README.md  

Fully compliant with Shodh’s submission requirements.

