# TelecomX_Challenge
TelecomX challenge for the Oracle Data Science program

Data analysis of the churn in clients for telecommunications from Latin America  using: **Python**, **Pandas** and **LightGBM**, This repository includes the Jupyter notebook with the workflow and process as well as the visualization of the data in multiple graphs.

---

## 📂 content

| File | Description |
|--------------|-------------|
| `TelecomX_LATAM.ipynb` | Main notebook with the Data, the set up, the cleaning process, exploratory analysis and predictive model training. |
| `Informe.md` | Findings and possible solutions presented to the client. |
| `app_churn.py` | Streamlit app that uses the procesed Dataset and the LightGBM model to explore the KPI's and clients within churn risk. |
| `TelecomX_Data.json` | Original Dataset in JSON format. |
| `requirements.txt` | Minimum requirements for the notebook and code to be properly run. |

---

## 1. Problem description.

Telecommunication companies face meaningful client loses due to churning. The main objective of this proyect is to understand the reasons behind it and create a model that predicts which clients have higher chances of leaving he company.


---

## 2. Workflow

1. * Pandas was used to read, flatten and normalize the JSON using 'pd.json_normalize', generating a 'flat_table' ready for analysis.*
  
2. * Transformation  of empty values to 'NaN' and changin the data types to the correct ones (float, int, etc).*
   * As this is a Latin America setting, the colummns we re renamed to spanish and the 'Churn' variable was turn into a binary (1= churned, 0 = active)*
   
3. * Exploratory analysis with KPI distribution and description.*
   * Churn visualization by gender, seniority, contract, payment method and internet service.*
   * critical segmentation: clients with over 12 months of seniority, month to month contracts, optic fiber and electronic payments/checks*
 
4. * Some of the key findings show that month to month clients have a 43% rate of churning. Electronic check seems to double the rate of churning compared to other payment methods such as credit cards and automatic payments.*
 
5. * a LightGMB model is trained with contractual, service and behaviour variables.*
   * The main KPI is 'ROC-AUC = 0.81' which can be configured (by default is set to 0.40).*
 
6. * Executive dashboard that allows real time KPI's, interactive graphics with Plotly and tabs for gender/seniority, fidelity, crosses, introduction and conclusions.*
   * The possibility to download CSV filed with the high churn risk clients identified by the model.*
 
---

## 3. How to execute locally

# 1. Clone or download the repository from: https://github.com/AlejandroEnciso7/TelecomX_Challenge

# 2. Open in a Python environment (Google colab or a code editor like VSCode)-

# 3. Install the dependencies found in the Requirements section.

# 4. Open the notebook.

# 5. Run the dashboard.


## 4. Credits

Developed by Alejandro Enciso
Contact: alejandroenciso6@gmail.com

---
