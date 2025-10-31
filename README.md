# 🧩 Employee Performance & HR Analytics Dashboard

## 📊 Project Overview
This project provides a comprehensive analysis of employee performance, salary, and HR-related indicators.  
It integrates multiple datasets — `FactEmployeePerformance`, `DimEmployee`, and `DimDepartment` — to uncover patterns, evaluate performance, and identify potential HR challenges.

The analysis aims to support **data-driven HR decision-making** by linking employee demographics, compensation, and performance metrics.

---

## 🎯 Objectives
- Evaluate performance and compensation across departments, cities, and genders.  
- Detect departments with **staffing or retention** issues.  
- Explore how **experience, attendance, and overtime** relate to performance.  
- Identify whether **salary, bonus, or tenure** affect employee outcomes.

---

## 🧰 Tools & Libraries
| Category | Tools Used |
|-----------|-------------|
| Data Analysis | **Python**, **Pandas**, **NumPy** |
| Visualization | **Matplotlib**, **Seaborn** |
| Date Handling | **Datetime**, **Timestamp** |
| Reporting | Jupyter Notebook, Markdown |

---

## 🧹 Data Preparation & Cleaning
### 1️⃣ Data Integration
- Merged:
  - `FactEmployeePerformance` 🧾 with `DimEmployee` on `EmployeeID`
  - Result merged with `DimDepartment` on `DepartmentID`

### 2️⃣ Data Cleaning
- Removed negative or null values in **Salary** and **Bonus**.
- Ensured all `EmployeeID` values exist across tables.
- Filled missing `PerformanceScore` and `AttendanceRate` with averages.
- Converted `Month` column to `datetime` format.

### 3️⃣ Feature Engineering
| Feature | Description |
|----------|-------------|
| `YearsAtCompany` | Calculated as `(Today - HireDate)` |
| `SalaryBand` | Categorized into Low, Mid, High |
| `AgeGroup` | Young (<30), Mid (30–45), Senior (>45) |
| `BonusRatio` | Derived from Bonus relative to Salary |
| `PerformanceRate` | Categorized as High / Low |

---

## ❓ Key Business Questions
1. What is the average performance score and salary per department?  
2. Which city has the highest average salary and bonus ratio?  
3. Are there gender differences in performance or bonus?  
4. How does years of service affect performance and salary?  
5. Which job title has the highest bonus ratio or best performance?  
6. How does salary range relate to performance score?  
7. Which age group performs best on average?  
8. Are employees with longer tenure more likely to get higher bonuses or performance?  
9. How do deductions, attendance, and overtime relate to performance?  
10. What are the employee status trends across departments?

---

## 🧠 Key Insights

### 🏢 Department Analysis
- **IT** department has the **highest average performance** (~3.09).  
- **Operations** offers **higher salaries** (~9,607) but **lowest performance** (~2.95).  
- Salaries are mostly balanced (~9,400–9,500) → fair pay structure.  
- Higher pay doesn’t guarantee better performance.

---

### 🏙 City Insights
- **Alexandria** has the **highest average salary**.  
- **Sohag** shows the **highest bonus average**.

---

### 👩‍💼 Gender Analysis
- **Females** slightly outperform **males** in performance.  
- **Males** receive higher **bonuses**, indicating possible imbalance in reward systems.

---

### 📆 Tenure & Experience
- Performance stays stable across service years with a small peak around **3 years**.  
- Salary increases are irregular → likely tied to **promotions**.  
- No direct correlation between tenure and bonus → reward system appears **performance-based**, not **experience-based**.

---

### 💼 Job Title Insights
- **Software Developers** have the **highest performance**.  
- **Marketing Coordinators** enjoy the **highest bonus average**.

---

### 💰 Salary Band & Age Group
- Performance consistent across salary bands.  
- **Senior employees** perform slightly better → experience adds value.  

---

### 📉 Deductions & Attendance
- Higher performers have **fewer deductions** and **better attendance**.  
- High performers work slightly **more overtime**, showing commitment.

---

### 🧍 Employee Status by Department
| Department | Key Insight |
|-------------|-------------|
| **HR** | Highest "On Leave" & lowest "Active" → Staffing issue |
| **IT** | Highest "Resigned" → Retention problem |
| **Finance** | Most "Active" employees → Stable department |
| **Customer Service** | Second-highest resignations → Attrition concern |
| **Operations** | Balanced distribution → Stable workflow |

---

## 📊 Example Visualizations
- **Performance vs Salary by Department**
- **Performance by Gender**
- **Salary Band vs Performance**
- **Years of Service vs Performance**
- **Bonus Ratio by Job Title**
- **Employee Status by Department**

*(Visuals created with Matplotlib & Seaborn)*

---

## 💡 Recommendations

### 1️⃣ HR & Retention
- Investigate **IT’s high resignation rate**; conduct stay interviews to understand causes.  
- Address **HR’s staffing gap** to maintain operational efficiency.  
- Implement wellness or flexibility programs to reduce attrition.

### 2️⃣ Pay & Bonus Policy
- Review **bonus allocation criteria** — ensure fair distribution between genders and departments.  
- Consider **performance-linked incentives** to better align pay with outcomes.

### 3️⃣ Training & Development
- Offer **skill-based training** to boost performance in low-performing departments (e.g., Operations).  
- Support early-career employees (0–3 years) to maintain their peak performance period.

### 4️⃣ Attendance & Productivity
- Reward consistent attendance and overtime contribution to sustain motivation.  
- Use deduction data to flag potential burnout or disengagement risks.

### 5️⃣ Strategic HR Insights
- Develop department-level KPIs using these findings.  
- Create **HR dashboards** to monitor real-time performance and engagement trends.


---

## 👨‍💻 Author
**Mostafa ElRkhawy**  
_Data Analyst | Python | Power BI | SQL | Excel_

📧 Contact: [LinkedIn Profile](www.linkedin.com/in/mostafa-elrkhawy) | [Gmail]((mostafaelrkhawy7@gmail.com))  
