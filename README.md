# OncoPilot


OncoPilot is an AI-powered precision medicine tool designed to predict how well cancer patients will respond to various chemotherapy drugs, using their tumor gene expression profiles. By leveraging public biomedical datasets, OncoPilot aims to reduce trial-and-error in cancer treatment and help oncologists make faster, data-driven drug decisions.


## Problem Statement

Chemotherapy is often prescribed using a one-size-fits-all approach. But patients can respond very differently to the same treatment. This leads to:

- Unnecessary toxicity
- Wasted time
- Increased mortality

OncoPilot bridges this gap using ML-based gene expression analysis to personalize chemotherapy recommendations.



## Solution Overview

Doctors or researchers can upload RNA-seq or microarray gene expression data to the platform. OncoPilot then:

- Analyzes the patient's gene expression
- Matches it with existing GEO/TCGA treatment response profiles
- Predicts which chemotherapy drugs are likely to be effective
- Visualizes ranked treatment options in an intuitive dashboard


## Datasets Used

- [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/)
- [TCGA](https://portal.gdc.cancer.gov/)
- [LINCS L1000](https://clue.io)
- [DrugBank](https://go.drugbank.com/)
- [PharmGKB](https://www.pharmgkb.org/)


## Tech Stack

| Layer              | Tools Used                         |
|--------------------|------------------------------------|
| Data Parsing       | GEOparse, Pandas                   |
| Preprocessing      | NumPy, Scikit-learn                |
| ML Models          | XGBoost, Logistic Regression       |
| Visualization      | Seaborn, Matplotlib, Plotly        |
| Web App            | Streamlit                          |
| Deployment Ready   | Docker, GitHub                     |


## Folder Structure

OncoPilot/
├── data/              # Sample GEO datasets
├── models/            # Trained ML models
├── webapp/            # Streamlit UI code
├── utils/             # Helper scripts (preprocessing, parsing)
├── README.md
├── requirements.txt

---

### How to Run

Basic usage instructions — shows you actually ran it.


1. Clone the repository:
```bash```
git clone https://github.com/NShenbagakrithika/OncoPilot.git
cd OncoPilot

2. Install dependencies 

pip install -r requirements.txt

3. Launch the streamlit app

streamlit run webapp/app.py


### Future Scope

- Expand support for additional cancer types
- Add drug toxicity prediction based on gene expression
- Integrate with hospital EMR systems
- Enable NLP-based clinical note integration for treatment planning

## Team

- Shenbaga Krithika N 
