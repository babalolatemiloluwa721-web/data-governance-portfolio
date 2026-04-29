# Data Governance Portfolio — Babalola Temiloluwa

Hands-on data governance project built using Microsoft Purview on Microsoft Azure. The project covers the full governance lifecycle for a real healthcare dataset from registering a data source to building a business glossary, classifying sensitive fields, and documenting data quality.

---

## About the Project

This portfolio implements a complete data governance framework for the Diabetes 130-US Hospitals dataset (1999–2008) — a real-world healthcare dataset containing 101,766 patient records across 130 US hospitals.

- **Dataset:** Diabetes 130-US Hospitals (1999–2008)
- **Source:** UCI Machine Learning Repository
- **Records:** 101,766 patient encounters
- **Columns:** 50 attributes
- **Governance Platform:** Microsoft Purview
- **Cloud Storage:** Microsoft Azure Blob Storage
- **Compliance Framework:** HIPAA
- **Data Owner & Steward:** Babalola Temiloluwa

---

## What Was Built

### 1. Data Source Registration
Registered the dataset as a governed asset in the Microsoft Purview Data Map, connected to Azure Blob Storage under the temi-governance-lab collection.

![Data Map](01_data%20map%20register.png)

### 2. Automated Metadata Scan
Configured and ran an automated scan (DiabetesScan01) to discover and catalog all dataset attributes and auto-classify sensitive fields.

![Scan In Progress](02%20scan%20in%20progress.png)

![Scan Completed](03_scan%20completed.png)

### 3. Azure Storage Container
Uploaded the diabetes dataset to Azure Blob Storage as the data source for the governance project.

![Azure Storage](06%20azure%20storage%20container.png)

### 4. Business Glossary
Created a Diabetes Dataset Glossary in Microsoft Purview with 5 approved terms linked directly to the data asset.

- **Patient Readmission** — A hospital admission occurring within 30 days of a previous discharge for the same or related condition
- **HbA1c Measurement** — A blood test measuring average blood sugar levels over 3 months, used to assess diabetes management quality
- **PII Data** — Personally Identifiable Information including age, gender and race requiring HIPAA compliance protection
- **Data Steward** — Person responsible for ensuring data quality, accuracy and compliance within a defined data domain
- **Discharge Status** — The condition and destination of a patient upon leaving the hospital facility

![Business Glossary Overview](04%20business%20glossary%20overview.png)

![Glossary Terms](05_glossary%20terms%20list.png)

### 5. Data Ownership and Stewardship
Assigned formal governance roles to the dataset asset in Microsoft Purview — Data Owner and Subject Matter Expert.

![Asset Contacts](07%20asset%20contacts%20owner.png)

### 6. Data Dictionary
Documented all 50 dataset columns covering data type, description, example values, sensitivity classification (High / Medium / Low), PII flagging, and HIPAA governance notes.

Sensitivity breakdown:
- **High** — PII/PHI fields: patient_nbr, race, gender, diag_1, diag_2, diag_3
- **Medium** — De-identified sensitive fields: age, weight, payer_code
- **Low** — Non-sensitive operational fields: all remaining columns

### 7. Data Governance Policy
Formal policy document covering data classification, access controls, HIPAA compliance, retention policy, and roles and responsibilities.

### 8. Data Quality Scorecard
Assessment of the dataset across five quality dimensions with field-level completeness analysis, validation rule results, and a remediation plan.

| Dimension | Score | Rating |
| --- | --- | --- |
| Completeness | 87% | Needs work |
| Accuracy | 91% | Good |
| Consistency | 94% | Good |
| Timeliness | 96% | Very good |
| Uniqueness | 98% | Very good |
| **Overall** | **93.2%** | **PASS** |

---

## Files in This Repository

- Diabetes Dataset Data Dictionary — Full 50-column data dictionary with classifications and governance notes
- Data_Governance Policy Temi Babalola.docx — Formal governance policy document
- Data Quality Scorecard_Temi Babalola.xlsx — Data quality assessment across 5 dimensions
- Screenshots — Evidence of Microsoft Purview implementation

---

## Tools Used

- Microsoft Purview — Data catalog, asset registration, glossary, classifications
- Microsoft Azure — Blob Storage, IAM, resource management
- Excel — Data dictionary documentation
- GitHub — Portfolio hosting and version control

---

## About

**Babalola Temiloluwa**

MS Management Information Systems — Texas Southern University (Dec 2026)

Data Governance | Data Quality | HIPAA Compliance | Microsoft Purview | SQL | Power BI

babalolatemiloluwa721@gmail.com
