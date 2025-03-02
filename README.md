# Maji Ndogo Water Services SQL Project

## Overview
The Maji Ndogo Water Services SQL Project is a comprehensive analysis of water infrastructure, employee performance, and contamination issues in the fictional region of Maji Ndogo. Built using MySQL and Jupyter notebooks, this project demonstrates advanced SQL querying, data analysis, and actionable insights for improving water services.

---

## Purpose
The purpose of this project is to:
- Analyze water infrastructure and identify areas for improvement.
- Detect discrepancies in employee performance and potential fraud.
- Provide actionable recommendations for improving water access and quality.
- Showcase SQL and data analysis skills in a real-world scenario.

---

## Tools and Technologies
- **Database**: MySQL
- **Programming**: Python, Jupyter Notebooks
- **Libraries**: `pandas`, `sqlalchemy`, `mysql-connector-python`, `ipython-sql`

---

## Features
- **Database Schema**: Fully structured `md_water_services` database with tables like `employee`, `water_source`, `visits`, and `global_water_access`.
- **Prebuilt Analysis**:
  - Infrastructure improvement recommendations.
  - Fraud detection workflows.
  - Provincial and town-level water access reports.
- **Reproducibility**:  Jupyter notebooks for easy replication.

---

## Key Insights
1. **Infrastructure Gaps**:
   - 45% of shared taps have queue times exceeding 30 minutes.
   - 15% of wells are contaminated and require immediate attention.
2. **Employee Performance**:
   - Top 3 employees conducted 60% of all visits.
   - Discrepancies were detected in 10% of employee-reported water quality scores.
3. **Fraud Detection**:
   - Identified 5 employees with above-average error rates.
   - Flagged 3 cases of potential bribery based on audit statements.

---

## Project Structure
```plaintext
├── data/                   # Contains sql data   
├── notebooks/              # Jupyter notebooks for analysis
├── Auditor_report.csv      # contains records of audits
├── .env.example            #Template for MySQL credentials
├── LICENSE                 # MIT license              
├── README.md               # Project overview and setup instructions
└── requirements.txt        # Python dependencies
```
---

## The following libraries are necessary for this project:
```plaintext
jupyterlab==4.0.4                 # For running interactive Python and SQL notebooks
mysql-connector-python==8.0.32    # For MySQL database connections
pandas==2.0.3                     # Data manipulation
sqlalchemy==2.0.20                # Database interactions
ipython-sql==0.5.0                # Run SQL queries in Jupyter notebooks
python-dotenv==1.0.0              # For loading environment variables
```
---

## Installation Instructions
 **Clone the Repository**:
   ```bash
   git clone https://github.com/JOEL-TAMAKLOE/maji-ndogo-water-service.git
   cd maji-ndogo-water-service
```
---
## Set-up
You can use any of the following approaches to set up and run the project:
1. ## For Quick Local Setup
  - This method is ideal for running the project locally without additional configuration.
  - Download and install MySQL from [mysql.com/downloads](https://dev.mysql.com/downloads/)
  - Run this command to load the database schema: mysql -u [USERNAME] -p < data/md_water_services.sql

  ## Note
  - In the notebooks, replace the placeholders ([USERNAME] and [PASSWORD]) in the SQL connection string with your local MySQL credentials:
  - %sql mysql+pymysql://[USERNAME]:[PASSWORD]@localhost:3306/md_water_services
  - Install Dependencies
  - pip install -r requirements.txt
  - Run Jupyter Lab

2. ## Using the .env File Method
- Copy the `.env.example` file, change the placeholders with your credentials, and rename it to .env
- Add .env to .gitignore to exclude it from version control.
- Install requirements and run jupyter lab

---

  ## Contribution Guidelines
Contributions are welcome! If you have improvement suggestions, please fork the repository and create a pull request. For major changes, please open an issue first to discuss what you would like to change
  
---
## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
