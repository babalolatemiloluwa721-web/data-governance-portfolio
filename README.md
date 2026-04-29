Data Governance Portfolio — Babalola Temiloluwa
> Hands-on data governance project demonstrating end-to-end implementation of enterprise data governance practices using **Microsoft Purview**, including data cataloging, metadata management, business glossary creation, data classification, and HIPAA-compliant asset stewardship.
---
📋 Project Overview
This portfolio project implements a complete data governance framework for the Diabetes 130-US Hospitals dataset (1999–2008) — a real-world healthcare dataset containing 101,766 patient records across 130 US hospitals. The project demonstrates core competencies required for a Data Governance Analyst role.
Detail	Info
Dataset	Diabetes 130-US Hospitals (1999–2008)
Source	UCI Machine Learning Repository
Records	101,766 patient encounters
Columns	50 attributes
Governance Platform	Microsoft Purview
Cloud Infrastructure	Microsoft Azure (Blob Storage)
Compliance Framework	HIPAA
Data Owner & Steward	Babalola Temiloluwa
---
🎯 Governance Objectives
Establish a centralised data catalog for a healthcare dataset
Classify and document sensitive PII and PHI fields in alignment with HIPAA requirements
Build a business glossary to standardise clinical and governance terminology
Assign data ownership and stewardship accountability
Document data lineage, quality rules, and metadata for all 50 columns
---
🛠️ Tools & Technologies
Tool	Purpose
Microsoft Purview	Data catalog, asset registration, glossary, classifications
Azure Blob Storage	Cloud storage for dataset
Microsoft Azure	Cloud infrastructure and IAM
Excel	Data dictionary documentation
GitHub	Portfolio hosting and version control
---
📁 Repository Structure
```
data-governance-portfolio/
│
├── README.md                          # Project overview (this file)
│
├── screenshots/                       # Evidence of Purview implementation
│   ├── 01_data_map_register.png       # Registered data source on Data Map
│   ├── 02_scan_in_progress.png        # Automated metadata scan running
│   ├── 03_scan_completed.png          # Successful scan completion
│   ├── 04_business_glossary.png       # Business glossary with 5 terms
│   ├── 05_glossary_terms_list.png     # All approved glossary terms
│   ├── 06_azure_storage.png           # Azure Blob Storage container
│   └── 07_asset_contacts.png          # Data catalog asset with glossary linked
│                                      # Data ownership and stewardship assigned
│
├── data-dictionary/
│   └── Diabetes_Dataset_Data_Dictionary_TemiBalabola.xlsx
│
├── governance-policy/
│   └── Data_Governance_Policy.docx    # Coming soon
│
└── data-quality/
    └── Data_Quality_Scorecard.xlsx    # Coming soon
```
---
✅ Phase 1 — Data Source Registration
Registered the Diabetes 130-US Hospitals dataset as a governed data asset in Microsoft Purview Data Map connected to Azure Blob Storage.
Key actions:
Created Azure Blob Storage account (`diabetesgovernance`)
Uploaded dataset to `diabetes-dataset` container
Configured Microsoft Purview Managed Identity with Storage Blob Data Reader role
Registered data source in Purview Data Map under `temi-governance-lab` collection
![Data Map](screenshots/01_data_map_register.png)
---
✅ Phase 2 — Automated Metadata Scan
Configured and executed an automated metadata scan (`DiabetesScan01`) to discover and catalog all dataset attributes.
Scan configuration:
Integration runtime: Azure AutoResolve
Credential: Microsoft Purview MSI (system)
Scan rule set: AzureStorage
Schedule: Manual (one-time)
![Scan Completed](screenshots/03_scan_completed.png)
---
✅ Phase 3 — Data Catalog & Asset Documentation
Registered the diabetes dataset as a formal data catalog asset with full governance documentation.
Asset documentation includes:
Professional asset description with HIPAA compliance context
Data hierarchy mapping: `diabetesgovernance` → `diabetes-dataset`
Collection path: `temi-governance-lab`
Assigned data owner and subject matter expert
![Asset Overview](screenshots/07_asset_overview.png)
---
✅ Phase 4 — Business Glossary
Created a Diabetes Dataset Glossary in Microsoft Purview with 5 approved governance and clinical terms linked directly to the data asset.
Term	Definition
Patient Readmission	A hospital admission occurring within 30 days of a previous discharge for the same or related condition
HbA1c Measurement	A blood test measuring average blood sugar levels over 3 months, used to assess diabetes management quality
PII Data	Personally Identifiable Information including age, gender and race requiring HIPAA compliance protection
Data Steward	Person responsible for ensuring data quality, accuracy and compliance within a defined data domain
Discharge Status	The condition and destination of a patient upon leaving the hospital facility
![Business Glossary](screenshots/04_business_glossary.png)
---
✅ Phase 5 — Data Ownership & Stewardship
Assigned formal data governance roles to the dataset asset in Microsoft Purview.
Role	Assigned To
Data Owner	Babalola Temiloluwa
Subject Matter Expert	Babalola Temiloluwa
![Contacts](screenshots/08_asset_contacts.png)
---
✅ Phase 6 — Data Dictionary
Documented all 50 dataset columns in a comprehensive data dictionary covering:
Column name, data type, and description
Example values
Sensitivity classification (High / Medium / Low)
PII flagging
HIPAA governance notes
Nullable status
Sensitivity breakdown:
🔴 High — PII/PHI fields: patient_nbr, race, gender, diag_1, diag_2, diag_3
🟡 Medium — De-identified sensitive fields: age, weight, payer_code
🟢 Low — Non-sensitive operational fields: all remaining columns
📥 Download Data Dictionary
---
🔜 Coming Soon
Data Governance Policy — formal policy document covering data classification, access controls, retention and HIPAA compliance
Data Quality Scorecard — completeness, accuracy and consistency metrics for the diabetes dataset
---
👤 About
Babalola Temiloluwa
MS Management Information Systems — Texas Southern University (Dec 2026)
Data Governance | Data Quality | HIPAA Compliance | Microsoft Purview | SQL | Power BI
📧 babalolatemiloluwa721@gmail.com
🔗 LinkedIn
---
This project was completed as part of a self-directed Data Governance Analyst portfolio building initiative, April 2026.
