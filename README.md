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
#### **Demographics**  
- **Gender**: 57.1% female, 42.9% male. Males were older (51.4 vs. 49.6 years, *p=0.020*).  
- **BMI**: Higher in males (27.5 vs. 25.5). Overweight prevalence: 46% males vs. 28.8% females.  
- **Smoking**: 23.7% males vs. 17.1% females were current smokers.  
- **Education**: More females held postgraduate degrees (18.4% vs. 15.7% males).  

#### **Clinical Tests**  
- **Blood Pressure**: Males had higher systolic (130.4 vs. 123.4 mmHg) and diastolic (80.8 vs. 76.0 mmHg) levels.  
- **Metabolic Markers**:  
  - Males: Higher glucose (99.5 mg/dL), uric acid (5.4 mg/dL), triglycerides (126.2 mg/dL).  
  - Females: Higher total cholesterol (201.1 mg/dL) and HDL (65.6 mg/dL).  

#### **Disease Prevalence**  
- **Hypertension**: 22.7% males vs. 12.6% females (*p<0.05*).  
- **Cardiovascular**: Myocardial infarction in 2.1% males vs. 0.3% females.  
- **Osteoporosis**: 10.7% females vs. 2.1% males (*p<0.05*).  

#### **Treatment**  
**Most Used Drugs**: Thyroxine, Metformin, Aspirin, Calcium, Rosuvastatin.  

---

---
