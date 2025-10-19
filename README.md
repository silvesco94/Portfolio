# Scott Silverstein Portfolio

<img src="profile_pic.jpg" alt="Scott Silverstein" style="width: 200px; display: inline-block; margin: 0;" />

### Email: scottsilverstein20@yahoo.com

### [Resume](silverstein%20resume.pdf)

### [LinkedIn](https://www.linkedin.com/in/scott-silverstein-69134498/)

## About Me
Hi! I am Scott Silverstein, a passionate data and business analytics professional with a strong foundation in programming, machine learning, and data-driven decision-making. Recently graduated with an MSBA in Business Analytics at the University of Utah, I bring a diverse educational background and professional experience to the table.

### **Education**
- **MSBA (Masters of Science in Business Analytics), Business Analytics** (2023 - 2024), University of Utah
- **BA, Comparative Politics with an Asian Studies emphasis** (2013 - 2017), University of Puget Sound
- **Certifications**:
  - Python Bootcamp (General Assembly, March 2023)
  - Salesforce Administration Certification (February 2023)
  - Marketing Analytics Certificate (Kellogg School of Business, March 2021)

### **Skills**
- **Programming & Cloud Platforms**: Python, R, SQL, AWS, Google Cloud, Pandas, Dask, Spark, Snowflake
- **Software**: Tableau, PowerBI, Excel, Salesforce
- **Machine Learning**: Neural Networks, Causal Modeling, Classification, Text Analytics, Synthetic Control
- **Other**: Data visualization, causal experiments, sequential testing, and Chinese language proficiency

### **Professional Experience**
With a track record of success in analytics-driven roles, I’ve managed over $8M in annual sales, optimized product placement strategies, and spearheaded transformative sales campaigns. My experience includes:
- Leveraging PowerBI and analytics to identify growth opportunities and improve profitability.
- Developing data-driven solutions in roles at Stanley Black & Decker, TTI, and EHealth Insurance.
- Applying analytical expertise to diverse sectors, from sales optimization to education.

Let’s explore my portfolio to see how I’ve applied my skills in real-world projects!

---

## Projects Overview

### [Capstone Projects](https://silvesco94.github.io/Swire-Cola-Capstone-/)
- **Predictive Maintenance Model for Swire Coca-Cola**: Developed a solution to minimize unplanned machine downtimes by forecasting machinery failures using survival analysis and machine learning models.
  - **Business Problem**: Addressed production shortfalls and estimated $60 million annual losses due to unplanned equipment breakdowns.
  - **Solution Approach**:
    - *Survival Analysis*: Estimated the likelihood of machine failures over time to predict high-risk periods.
    - *Random Forest Models*: Identified key features influencing breakdowns, providing accurate predictions.
    - *Logistic Regression*: Predicted probabilities of equipment failure under specific conditions.
  - **Business Value**:
    - *Proactive Maintenance Planning*: Reduced unplanned downtimes by identifying high-risk machinery, improving repair efficiency and resource allocation.
    - *Operational Efficiency*: Enhanced production continuity, meeting customer demands through consistent schedules.
    - *Cost Savings*: Aimed to cut downtime-related losses by at least 50%, potentially saving millions annually.
  - **Challenges Overcome**:
    - Managed over 80% missing equipment IDs, reducing model granularity at the machine level.
    - Handled imbalanced breakdown data to avoid overfitting.
    - `Addressed inconsistent date fields through extensive preprocessing for accurate analysis.`

---
### [Credit Default Risk](https://silvesco94.github.io/home_credit/) 


- **Work Project:** End-to-end credit-risk modeling to predict applicant default probability and guide underwriting.

- **Business Problem:** Expand responsible lending while keeping portfolio risk within target bounds; primary KPI = ROC–AUC (with calibration and lift by decile as secondary).

- **Solution Approach:**
  - *EDA & Data Quality:* missingness, leakage screening, and encoding; class-imbalance assessment.
  - *Models:* regularized logistic regression baseline; gradient-boosted trees (XGBoost) for non-linear signal.
  - *Validation:* stratified k-fold CV, held-out test, cost-aware threshold tuning; calibration checks.
  - *Explainability:* permutation importance and partial-dependence style diagnostics.

- **Business Value:**
  - *Risk Control:* higher AUC and strong lift in high-risk deciles improve approval/decline decisions.
  - *Inclusion:* enables approving more low-risk borrowers without increasing defaults.
  - *Operationalization:* clear operating threshold plus monitoring plan for drift and fairness.

- **Challenges Overcome:**
  - Managed severe class imbalance and correlated features without leakage.
  - Standardized categorical encodings; consolidated redundant signals.
  - Delivered stakeholder artifacts: problem statement, EDA report (HTML), reproducible R Markdown pipeline, and a findings deck.

---
### [Machine Learning](https://silvesco94.github.io/Machine-Learning/)
- Developed advanced machine learning models for tasks like classification, clustering, and regression.
- Applied techniques such as neural networks, ensemble models, and support vector machines to solve real-world problems.
- `Highlighted by a capstone project analyzing salary fairness in Major League Baseball using predictive models and clustering techniques.`

---

### [Data Engineering](https://silvesco94.github.io/Data-Engineering/)
- **Baseball Stats Pipeline**:
  - Automated data collection using the Pybaseball package and APIs like Fangraphs and MLB.
  - Designed a relational database schema (3NF) and used GCP for scalable storage.
  - Built Airflow workflows for automated data ingestion and updates.
- **ETL Pipeline**:
  - Extracted, transformed, and loaded data into structured formats using Python and SQL.
  - Standardized data to ensure compatibility with the database schema.
- **Challenges and Future Plans**:
  - Resolved inconsistent player IDs across sources and refined schema design.
  - `Plan to integrate additional datasets and optimize querying with advanced storage solutions.`

---

### [Data Mining](https://silvesco94.github.io/Data-Mining/)
- Explored data patterns through clustering, association rule mining, and decision tree classification.
- Implemented algorithms like K-Means and Apriori to derive actionable insights.
- `Evaluated model performance using metrics like silhouette scores and feature importance.`

---

### [Causal Modeling](https://silvesco94.github.io/Causal-Experiments/)
- Explored causal relationships through experiments and observational data.
- Applied techniques like A/B testing, propensity score matching, and synthetic controls.
- Focused on actionable insights for decision-making and policy evaluation.

---

### [Database Design for University of Utah Health](https://silvesco94.github.io/Utah-Health-Database/)

- **Project Overview**: Designed a fully relational **Hospital Management System (HMS)** using SQL for the University of Utah Health. The database enables secure management of patients, doctors, billing, laboratory tests, and telehealth data — ensuring HIPAA compliance and efficient data retrieval.

- **Business Problem**: Existing healthcare data systems often suffer from fragmented storage and poor interoperability. This project addresses those issues by creating a **centralized SQL database** that supports secure, real-time information sharing between doctors, patients, and administrators.

- **Solution Approach**:
  - **SQL Schema Design**: Built normalized schemas (3NF) for core hospital entities — `Hospital`, `Patient`, `Doctor`, `Appointment`, `Billing`, and `Pharmacy`.
  - **Referential Integrity**: Defined primary and foreign key relationships to ensure accurate linkages and enforce cascading updates.
  - **Mock Data Generation**: Used **Mockaroo** to populate 15 interconnected tables with realistic synthetic healthcare data.
  - **Role-Based Access Control (RBAC)**: Created a `user_table` with role hierarchy for secure access aligned with HIPAA standards.
  - **Telehealth Extension**: Added `TelehealthAppointment` and `TelehealthFeedback` tables to support modern virtual healthcare operations.

- **Business Value**:
  - **Operational Efficiency**: Streamlined appointment scheduling, billing, and inventory management in one SQL-backed system.
  - **Data Consistency**: Improved data accuracy through normalized table structures and constraint-driven validation.
  - **Scalability**: Database design supports new departments, clinics, and patient types without altering core schema.
  - **Compliance**: Integrated encryption-ready fields and role-based data segregation for HIPAA alignment.

- **Challenges Overcome**:
  - Addressed referential integrity conflicts between dependent tables.
  - Ensured schema normalization without redundancy across 15+ tables.
  - Validated foreign key dependencies and cross-table joins using test queries.
  - Balanced data realism and security through synthetic record generation.
 
    
---

### [War Games — Baseball Analytics Blog](https://silvesco94.github.io/war_games/)

- **Project Overview**: Co-authored and developed a data-driven **baseball analytics blog** focused on modern sabermetric insights and statistical modeling. The site is hosted through **GitHub Pages** and designed as a modular content hub linking multiple analysis repositories, each representing an independent research article.

- **Purpose**: To translate advanced baseball statistics into accessible, visual narratives. Each post blends data science with storytelling — integrating Python-based analytics, player performance models, and MLB data pipelines to make analytics approachable for a broader baseball audience.

- **Technical Stack**:
  - **Python / Pandas / NumPy** for data cleaning, modeling, and feature engineering  
  - **Matplotlib / Seaborn** for visualization and chart creation  
  - **GitHub Pages (Jekyll)** for static site hosting and layout customization  
  - **Markdown / HTML** for article formatting and inline chart display  
  - **Git Workflow** to manage version control and collaborative publishing  

- **Structure & Workflow**:
  - Each article is its own GitHub repository, containing notebooks, scripts, and graphics.  
  - The **central repository** acts as the homepage, hosting:
    - `index.md` (site index linking to articles)  
    - `_config.yml` (site and theme settings)  
    - `assets/images/` (article thumbnails)  
  - Articles are linked with metadata, author credits, and preview images for a professional blog experience.

- **Analytics Focus**:
  - **WAR (Wins Above Replacement)** and **wRC+** analysis for measuring player efficiency.  
  - **Pitch-level modeling** using Statcast data to explore approach, contact quality, and expected outcomes.  
  - **Salary fairness and performance regression studies** — examining how statistical output aligns with player compensation.  
  - **Interactive visualization-ready datasets**, prepared for future integration with dashboards or advanced statistical tools.

- **Business Value**:
  - **Knowledge Sharing**: Bridges academic-level analytics with fan-level accessibility.  
  - **Scalability**: Blog structure allows continuous growth — each new repo is a new “chapter” of analysis.  
  - **Collaboration**: Encourages co-authorship and contribution from other data scientists and analysts.  
  - **Professional Branding**: Demonstrates technical writing, visualization, and analytical storytelling skills to potential employers.

- **Challenges Overcome**:
  - Designed a **Git-backed publishing system** to manage multiple repositories under one live domain.  
  - Managed **rendering consistency** across articles with different markdown and Jupyter formats.  
  - Optimized image paths and `_config.yml` for compatibility with GitHub Pages’ static rendering.  
  - Balanced visual design, narrative clarity, and advanced analytics within a lightweight static site.



---

## Thank You
Thank you for taking the time to explore my portfolio! Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/scott-silverstein-69134498/) or reach out to discuss potential collaborations and opportunities.
