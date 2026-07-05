# Heart-Failure-Clinical-Records-Dashboard-V1
Machine learning project analyzing heart failure clinical records to predict patient mortality risk. Includes data preprocessing, exploratory data analysis, feature engineering, and model evaluation for clinical risk stratification.

## Dataset
@article{Chicco2020MachineLC,
  title={Machine learning can predict survival of patients with heart failure from serum creatinine and ejection fraction alone},
  author={Davide Chicco and Giuseppe Jurman},
  journal={BMC Medical Informatics and Decision Making},
  year={2020},
  volume={20},
  url={https://api.semanticscholar.org/CorpusID:211018036}
}

This project uses the Heart Failure Clinical Records Dataset, which contains medical records of 299 patients collected at the Faisalabad Institute of Cardiology and the Allied Hospital in Faisalabad, Pakistan, between April and December 2015. The cohort includes 194 male and 105 female patients, aged between 40 and 95 years. All patients had left ventricular systolic dysfunction and had experienced previous heart failure classified as NYHA class III or IV, indicating advanced-stage heart failure.

The dataset consists of 13 clinical, physiological and lifestyle-related features, including both numerical and binary variables. Binary variables include anaemia, high blood pressure, diabetes, sex, and smoking status. Clinical measurements capture key biomarkers relevant to cardiovascular and organ function, such as:
  - Creatinine phosphokinase (CPK): an enzyme indicating potential muscle or cardiac injury when elevated
  - Ejection fraction: percentage of blood pumped out of the left ventricle per heartbeat, a key measure of cardiac function
  - Serum creatinine: an indicator of kidney function, with elevated levels suggesting renal impairment
  - Serum sodium: electrolyte levels associated with fluid balance and may be affected in heart failure patients
The target variable is death event, representing patient survival status during an average follow-up period of 130 days. 

This dataset is commonly used for binary classification tasks, particularly in predicting mortality risk in heart failure patients, and is well-suited for machine learning applications in clinical risk stratification.
