# 📊 IBM HR Analytics: Employee Attrition & Retention Analysis

An executive-level Exploratory Data Analysis (EDA) project analyzing the IBM HR Employee Attrition dataset. This analysis investigates key behavioral, financial, and demographic drivers behind employee turnover—such as overtime workload, early-career tenure risks, stock option distribution, and compensation gaps—to provide actionable retention strategies for HR leadership.

---

## 📌 Business Problem & Executive Overview

Employee attrition presents significant operational and financial challenges, including recruitment costs, lost productivity, and diminished team morale. By transitioning from reactive exit interviews to proactive data analysis, HR teams can pinpoint the root causes of resignation and implement targeted retention strategies.

---

## 📁 Repository Structure

```text
├── data/                                         # Raw and processed IBM HR dataset
├── EDAQuestions/                                 # Business analytical questions & research framework
├── Report/                                       # Executive presentation slides & report documents
├── plots/                                        # Generated EDA visualization charts
│   ├── Percentage of Missing values.png
│   ├── Distribution of Age.png
│   ├── Distribution of MonthlyIncome.png
│   ├── Distribution of DistanceFromHome.png
│   ├── TotalWorkingYears Distribution.png
│   ├── YearsAtCompany Distribution.png
│   ├── YearsWithCurrManager Distribution.png
│   ├── Attrition Distribution.png
│   ├── Gender Distribution.png
│   ├── Department Distribution.png
│   ├── JobRole Distribution.png
│   ├── OverTime Distribution.png
│   ├── BusinessTravel Distribution.png
│   ├── Employee Attrition Count by Department.png
│   ├── Employee Attrition Count by JobRole.png
│   ├── Employee Attrition Count by OverTime.png
│   ├── Employee Attrition Count by BusinessTravel.png
│   ├── Employee Attrition Count by AgeGroup.png
│   ├── Employee Attrition Count by MaritalStatus.png
│   ├── Monthly Income Distribution Leavers vs Stayers.png
│   ├── TotalWorkingYears Distribution Stayers vs Leavers.png
│   ├── Years At Company Distribution Stayers vAs Leavers.png
│   ├── Attrition Rate (%) by Commute Distance Group.png
│   ├── Attrition Count by YearsInCurrentRole.png
│   ├── Attrition Rate (%) by Stock Option Level.png
│   └── Attrition Count by Gender.png
├── IBM_HR_Analytics_Employee_Attrition_Analysis.ipynb # Primary Jupyter notebook with EDA code
└── README.md                                     # Project documentation
```

---

## 🔑 Key Insights & Findings

* **Overall Attrition Baseline:** 
  * Retained employees represent **83.99%** (1,264) of the dataset, while **16.01%** (241) have left the organization[cite: 2].
  * The dataset exhibits a **5:1 class imbalance** between retained and left employees[cite: 2].

* **Demographics & Early-Career Flight Risk:**
  * **Single employees** (**25.10%** attrition) and **young employees aged 18–30** (**25.90%** attrition) show significantly elevated turnover compared to older or married peers.

* **Compensation & Salary Impact:**
  * **Low-Income Vulnerability:** Over 75% of attrited employees earn under **$6,000/month**, with a median income of **~$3,200** vs. **~$5,200** for stayers.
  * **Stock Option Level:** Employees without stock options (Level 0) leave at the highest rate (**24.4%**), whereas offering moderate equity (Levels 1 & 2) cuts attrition to **7.5%–9.2%**.

* **Workload & Burnout Factors:**
  * **Overtime:** **28% of the workforce** (422 employees) works overtime, posing a major risk factor for burnout and turnover.

---

## 💡 Strategic Recommendations for HR Leadership

1. **Early-Career Engagement:** Establish targeted mentorship programs, structured career pathways, and competitive entry packages for young employees (aged 18–30).
2. **Review Junior Base Salaries:** Re-evaluate compensation bands for entry and mid-level roles earning under $6,000/month to prevent loss to market competitors.
3. **Expand Equity Distribution:** Extend Level 1 stock option eligibility to mid-level roles to leverage its strong retention effect.
4. **Cap Overtime Dependency:** Audit workload distributions in high-overtime departments to mitigate burnout-driven exits.

---

## 🛠️ How to Run This Project

1. **Clone the repository:**
   ```bash
   git clone https://github.com/kalpitkishore/IBM-HR-Analytics-Employee-Attrition.git
   cd IBM-HR-Analytics-Employee-Attrition
   ```

2. **Install required dependencies:**
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

3. **Launch the Notebook:**
   Open `IBM_HR_Analytics_Employee_Attrition_Analysis.ipynb` inside VS Code or Jupyter Notebook to run the interactive analysis.