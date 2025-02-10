**Cyprus Biobank Data Analysis**  
**Project: Analysis of 1346 Participants' Demographic and Medical Data**  

---

### **Overview**  
This Jupyter notebook analyzes data from 1,346 participants in the Cyprus Biobank study. The analysis focuses on demographic characteristics, medical history, and biochemical measurements, leveraging Python libraries for statistical summaries, visualizations, and hypothesis testing.

---

### **Dataset**  
**File:** `cyprus_1346_participants.csv`  
**Variables Included:**  
- **Demographics**: Age, Sex, Family Status, Education Level, Smoking Habits, etc.  
- **Medical History**: Hypertension, Asthma, Diabetes, Cancer, Drug Use, etc.  
- **Biochemical Measurements**: Blood Pressure, BMI, Glucose, Cholesterol, Triglycerides, etc.  
- **Lab Results**: Leukocytes, Erythrocytes, Hematocrit, and more.  

---

### **Key Analyses**  
1. **Descriptive Statistics**  
   - Continuous variables (Age, Height, Weight, BMI) summarized using `pandas.describe()`.  
   - Categorical variables (Sex, Smoking, Education Level) analyzed via frequency counts and percentages.  

2. **Visualizations**  
   - Heatmaps and boxplots (e.g., BMI vs. Blood Pressure).  
   - Distribution plots for variables like Age and Glucose levels.  

3. **Statistical Testing**  
   - Chi-square tests for categorical variables (e.g., Smoking vs. Hypertension).  
   - T-tests for group comparisons (e.g., Healthy Cohort vs. Diseased).  

4. **Clinical Summary Tables**  
   - Generated using the `tableone` library to produce publication-ready descriptive tables.  

---

### **Dependencies**  
- Python Libraries:  
  ```bash
  pandas, numpy, matplotlib, seaborn, scipy, tableone
  ```  
- Install dependencies:  
  ```bash
  pip install tableone pandas numpy matplotlib seaborn scipy
  ```

---

### **Code Structure**  
1. **Data Loading**  
   - Load the dataset and list columns.  
2. **Demographic Analysis**  
   - Summary statistics for continuous variables.  
   - Frequency counts for categorical variables.  
3. **Visualizations**  
   - Heatmaps, boxplots, and histograms.  
4. **Statistical Analysis**  
   - Chi-square and t-tests for group comparisons.  
5. **TableOne Output**  
   - Generate a clinical summary table.  

---

### **Key Findings**  
- **Demographics**: Majority of participants were married (72.7%), with a mean age of 50.4 years.  
- **Smoking**: 19.9% were current smokers, 10.6% former smokers.  
- **Medical Conditions**: 56.1% had a prior medical diagnosis; 20.9% reported hypertension.  
- **Biochemical Trends**: Mean BMI was 26.35 (overweight range), with notable correlations between BMI and blood pressure.  

---
