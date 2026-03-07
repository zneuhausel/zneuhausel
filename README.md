# 👋 Hi, I'm [Zoe]

## 🧠 Soft Skills
![Analytical Thinking](https://img.shields.io/badge/Analytical%20Thinking-4A90D9?style=for-the-badge)
![Critical Thinking](https://img.shields.io/badge/Critical%20Thinking-5B7FA6?style=for-the-badge)
![Intellectual Curiosity](https://img.shields.io/badge/Intellectual%20Curiosity-6B6FA6?style=for-the-badge)
![Risk & Strategic Thinking](https://img.shields.io/badge/Risk%20%26%20Strategic%20Thinking-7B5FA6?style=for-the-badge)
![Problem-Solving](https://img.shields.io/badge/Problem--Solving%20Persistence-8B4FA6?style=for-the-badge)

## 🛠️ Hard Skills

**Languages & AI**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![NLP](https://img.shields.io/badge/NLP-Natural%20Language%20Processing-76B900?style=for-the-badge&logo=openai&logoColor=white)

**Data & Databases**

![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Databases](https://img.shields.io/badge/Databases-336791?style=for-the-badge&logo=postgresql&logoColor=white)

**Research & Workforce Tools**

![SPSS](https://img.shields.io/badge/SPSS-052FAD?style=for-the-badge&logo=ibm&logoColor=white)
![Lightcast](https://img.shields.io/badge/Lightcast-FF4B00?style=for-the-badge)
![Policy Analysis](https://img.shields.io/badge/Research%20%26%20Policy%20Analysis-2E7D32?style=for-the-badge)
![Labor Market Data](https://img.shields.io/badge/Labor%20Market%20%26%20Workforce%20Data-1565C0?style=for-the-badge)



# 📁 Projects

---

## 🏥 Field Hospital Optimization — COVID-19 Response Planning
**Type:** Collegiate | **Tools:** Python, Pyomo, Pandas, Google Colab

### 🔍 Business Problem
A Canadian company based in Marystown, Newfoundland was contracted to produce field hospitals during the COVID-19 pandemic. With limited labor across three departments (A, B, and C) and only 50 employees available over an 8-week window, the company needed to determine:
- How many **small** (50-patient) vs. **large** (300-patient) hospitals to build
- How to **optimally assign employees** to departments to maximize patient capacity
- All while respecting mix constraints: at least 20% small hospitals, at least 60% large hospitals

### 🛠️ What I Did
Built a full **Integer Programming (IP) optimization model** from scratch using Python and Pyomo:
- Loaded and structured real input data from Excel using Pandas
- Formulated decision variables for both hospital counts and employee-department assignments
- Defined a patient-maximization objective function (non-monetary)
- Encoded all business constraints: labor hour limits, hospital mix ratios, and employee eligibility rules
- Solved using the HiGHS solver and validated the optimal solution

### ⚠️ Challenges
- Shifting from a cost-minimization mindset to a **patient-maximization** objective required rethinking the model structure
- Modeling **flexible employees** (those eligible for multiple departments) required a two-dimensional variable and careful constraint logic to ensure every employee was fully assigned
- Ensuring integer (whole number) solutions while meeting all constraints simultaneously

### 📊 Results & Business Impact
The model returned an optimal solution of **29,900 patients served**, recommending:
- **95 large hospitals** and **28 small hospitals** built
- All 50 employees fully assigned to their eligible departments with zero waste
- The mix constraints satisfied — ensuring both operational efficiency and contractual compliance

This analysis gives the company a **data-driven deployment plan** that maximizes healthcare reach during a crisis, supporting faster and more equitable COVID-19 response.

### 🔗 Artifacts
- 📓 [View Notebook on GitHub](#your-repo-link-here)
