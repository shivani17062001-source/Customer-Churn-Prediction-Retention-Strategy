ChurnRx: Telco Customer Churn Analysis and Retention Strategy

🚀 Why ChurnRx?
In the competitive telecom world, customer churn can cost millions. What if you could predict who's about to leave and stop them with targeted strategies? ChurnRx is your prescription for retention success! This open-source project analyzes the Telco Customer Churn dataset to uncover hidden patterns, visualize key insights, and deliver actionable retention tactics. Built for data enthusiasts, analysts, and business leaders, it's easy to run in Google Colab—no heavy setup required. Dive in, explore churn drivers, and transform data into loyalty! 📊💡

📋 Project Overview
ChurnRx leverages Exploratory Data Analysis (EDA) on a real-world telecom dataset (~7,000 customer records) to identify why customers leave. Features include demographics (e.g., gender, SeniorCitizen), services (e.g., InternetService, Contract), and billing (e.g., MonthlyCharges, TotalCharges). The binary Churn target (Yes/No) helps pinpoint at-risk groups.

Key highlights:

Churn Rate: ~26% overall—address it before it bites!
Data Source: Telco Customer Churn Dataset from Kaggle.
Tech Stack: Python (pandas, seaborn, matplotlib, scipy) in Google Colab.

✨ Features

Data Cleaning & Preparation: Handles missing values, converts data types, and encodes categoricals for seamless analysis.
Exploratory Data Analysis (EDA):

Univariate: Histograms and countplots to spot distributions and imbalances.
Bivariate: Countplots and boxplots revealing churn by contract type, services, and charges.
Correlations: Heatmap showing relationships (e.g., longer tenure = lower churn).
Statistical Tests: Chi-squared to validate significant churn predictors.


Visualizations: Engaging plots with plt.tight_layout() for clean layouts—perfect for reports!
Retention Strategies: Actionable insights like promoting long-term contracts and senior discounts.
Extensibility: Ready for ML models (e.g., Logistic Regression, Random Forest) to predict churn.

🛠️ Installation & Setup
No local install needed—run it in the cloud!

Open in Colab: Click the badge above or visit Google Colab and upload the notebook.
Download Dataset:

Head to Kaggle.
Download WA_Fn-UseC_-Telco-Customer-Churn.csv.


Upload to Colab:

In Colab, use the left sidebar Files panel to upload the CSV.
Or run:
pythonfrom google.colab import files
uploaded = files.upload()  # Select the CSV file



Dependencies: All libraries (pandas, numpy, matplotlib, seaborn, scipy) are pre-installed in Colab. No extras required!

📖 Usage

Load the dataset: df = pd.read_csv('WA_Fn-UseC_-Telco-Customer-Churn.csv').
Run the code cells sequentially for cleaning, EDA, visualizations, and insights.
Explore outputs: Heatmaps, plots, and printed strategies.
Customize: Add your own ML models or tweak visuals.

Example snippet for correlation heatmap:
pythoncorr_matrix = df_encoded.corr()
plt.figure(figsize=(12, 10))
sns.heatmap(corr_matrix, annot=False, cmap='coolwarm')
plt.title('Correlation Matrix Heatmap')
plt.tight_layout()
plt.show()
🔍 Key Insights & Retention Strategies

High-Risk Groups: Month-to-month contracts (~40% churn), fiber optic users, seniors (~10% higher churn).
Strategies:

🎁 Offer discounts for 1-2 year contracts.
⚙️ Enhance fiber optic reliability with bundles.
👴 Senior perks: Tailored plans and support.
💸 Rebates for high MonthlyCharges (> $70).
👋 Onboarding programs for new customers (low tenure = high churn).



Prioritize Contract, tenure, and Internet Service for maximum impact!
🤝 Contributing
We welcome contributions! Fork the repo, make changes, and submit a pull request. Ideas:

Add ML prediction models.
Enhance visualizations (e.g., interactive plots with Plotly).
Test with new datasets.

Follow the Code of Conduct. Questions? Open an issue!

👨‍💼 Author
Shivani Uppala
Business Analyst with 4 years of experience bridging business needs and technical solutions across logistics, manufacturing, and financial services. Skilled in requirements gathering, BPMN process modeling, and impact analysis, with a proven record of driving process improvements through Lean Six Sigma and Kaizen methodologies. Proficient in SQL, Power BI, Tableau, and cloud platforms (AWS, Azure, GCP, Snowflake) to deliver data-driven insights and automation. Adept at stakeholder engagement, Agile methodologies, and compliance frameworks (SOX, HIPAA, AML), with strong analytical, problem-solving, and communication skills that consistently improve efficiency and business outcomes.
LinkedIn Profile | 📧 Shivaniuppala034@gmail.com | ☎️ (475) 287-3249

📜 License
This project is licensed under the MIT License—see LICENSE for details.
