import os

# Content for the README.md file based on the user's project details
readme_content = """# SAP FI Record-to-Report (R2R) Process Design
## Capstone Project: Month-End Financial Close Simulation

### Project Overview
This repository contains the Capstone Project documentation for a complete **Record-to-Report (R2R)** cycle designed in **SAP Financial Accounting (FI)**. The project simulates the financial operations of **VishTech Manufacturing Pvt. Ltd.**, a fictitious industrial equipment manufacturer based in Bhubaneswar, India.

### Objective
The primary goal of this project is to demonstrate how SAP ERP transforms manual, error-prone month-end closing processes into an automated, auditable, and efficient workflow compliant with **Indian Accounting Standards (Ind AS)** and the **Companies Act 2013**.

### Tech Stack
* **ERP Platform:** SAP ECC 6.0 / SAP S/4HANA
* **SAP Module:** FI (Financial Accounting)
* **Sub-Modules:** General Ledger (FI-GL), Asset Accounting (FI-AA)
* **Fiscal Year Variant:** V3 (April - March | Indian Financial Year)
* **Company Currency:** INR (Indian Rupee)
* **Reporting Tool:** SAP Financial Statement Version (FSV)

### Key SAP Transactions (T-Codes)
| Step | Process Description | T-Code |
| :--- | :--- | :--- |
| 1 | SAP System Navigation | SAP1 |
| 2 | Company Code Configuration | OX02 |
| 3 | Chart of Accounts Setup | OB13 |
| 4 | Month-End Journal Entry Posting | FB50 |
| 5 | Asset Depreciation Run | AFAB |
| 6 | Financial Statement Generation | F.01 |

### Project Repository Structure
* `/Documentation`: Contains the final 5-page Capstone Project PDF report.
* `README.md`: Project summary and technical overview.

### Author
* **Name:** Vishakha Sah
* **Roll Number:** 23053585
* **Program:** B.Tech, Computer Science and Engineering
* **Institution:** Kalinga Institute of Industrial Technology (KIIT), Bhubaneswar

### Declaration
This is an original, individual submission. Screenshots provided in the documentation are sourced from SAP IDES reference systems for simulation purposes as live SAP credentials were unavailable. All process design and analysis have been prepared independently.
"""

# Define the output path
output_path = '/mnt/data/README.md'

# Write the content to the file
with open(output_path, 'w') as f:
    f.write(readme_content)

print(f"README.md file generated successfully at {output_path}")
