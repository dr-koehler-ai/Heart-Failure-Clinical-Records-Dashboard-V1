# Clinical Background and Initial Hypotheses

Before performing the exploratory data analysis (EDA), several clinical hypotheses were formulated based on existing medical knowledge. Defining hypotheses prior to data exploration helps reduce confirmation bias and provides a structured framework for interpreting the results.

---

## Expected Prognostic Factors

Based on clinical experience, the following variables were expected to have the strongest association with mortality:

### 1. Ejection Fraction

Ejection fraction (EF) is a key indicator of cardiac systolic function. A reduced EF reflects impaired ventricular pumping capacity and is associated with advanced heart failure, cardiogenic shock, and poor clinical outcomes.

**Hypothesis:** Lower ejection fraction is associated with increased mortality.

---

### 2. Serum Creatinine

Elevated serum creatinine reflects impaired renal function. In patients with heart failure, worsening kidney function is frequently associated with advanced disease and the development of cardiorenal syndrome.

**Hypothesis:** Higher serum creatinine levels are associated with increased mortality.

---

### 3. Age

Advanced age is generally associated with reduced physiological reserve, greater frailty, and a higher prevalence of comorbidities, all of which contribute to poorer outcomes in heart failure.

**Hypothesis:** Older patients have a higher risk of mortality.

---

## Variables Expected to Have a Moderate Association

Several additional variables were expected to influence mortality, although their prognostic value may be weaker or mediated through other clinical conditions.

### Anaemia

Reduced haemoglobin levels decrease oxygen transport capacity and may reflect chronic disease, nutritional deficiencies, or occult bleeding.

**Hypothesis:** Anaemia is associated with higher mortality.

---

### Platelets

Abnormal platelet counts may indicate systemic illness, inflammation, bleeding disorders, or bone marrow dysfunction.

**Hypothesis:** Abnormal platelet levels may be associated with mortality, although the relationship is expected to be weaker than for cardiac or renal function markers.

---

### Serum Sodium

Hyponatraemia is frequently observed in advanced heart failure and often reflects neurohormonal activation and disease severity.

**Hypothesis:** Lower serum sodium levels are associated with increased mortality.

---

### Creatinine Phosphokinase (CPK)

Elevated CPK levels indicate tissue damage, particularly skeletal muscle injury, but may also increase following myocardial injury.

**Hypothesis:** Higher CPK values may be associated with increased mortality.

---

### Diabetes

Diabetes mellitus accelerates vascular disease and contributes to chronic kidney disease, increasing overall cardiovascular risk.

**Hypothesis:** Patients with diabetes have a higher mortality risk.

---

### High Blood Pressure

Hypertension is a major cardiovascular risk factor and contributes to structural heart disease.

**Hypothesis:** Hypertension may be associated with mortality, although its effect could be attenuated after heart failure has developed.

---

### Smoking

Smoking accelerates atherosclerosis and coronary artery disease while reducing cardiovascular reserve.

**Hypothesis:** Smokers may experience higher mortality than non-smokers.

---

### Sex

Sex-specific differences exist in the clinical presentation and progression of cardiovascular disease.

**Hypothesis:** Mortality may differ between male and female patients; however, this relationship may be confounded by differences in age, comorbidities, and cardiovascular risk factors.

---

## Expected Relationships

Based on clinical reasoning, several variables are unlikely to exhibit a purely linear relationship with mortality.

For example:

- Mortality may increase disproportionately at very high serum creatinine levels.
- Very low ejection fractions may be associated with a steep increase in mortality risk.
- Advanced age may show an accelerating rather than linear increase in mortality.

These assumptions will be evaluated during the exploratory data analysis.

---

## Considerations for Predictive Modelling

The variable **`time`** represents the patient's follow-up duration.

Although useful for descriptive analyses, this variable would not be available when predicting mortality at the time of hospital admission.

Therefore, it would introduce **data leakage** if included in a predictive machine learning model and should be excluded from models intended for prospective clinical risk prediction.
