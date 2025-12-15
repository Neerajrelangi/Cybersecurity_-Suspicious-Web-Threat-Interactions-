🔐 Cybersecurity: Suspicious Web Threat Interactions
📊 Project Overview
This project focuses on analyzing web traffic data collected from AWS CloudWatch to detect suspicious and potentially malicious web interactions. The goal is to help organizations identify abnormal traffic patterns and possible cyber attack attempts on cloud-hosted applications. Using data analysis and machine learning techniques, the project performs exploratory data analysis (EDA), anomaly detection, and classification modeling to automate the identification of security threats in web traffic.
📂 Dataset
File: CloudWatch_Traffic_Web_Attack.csv
Records: 282
Features: 16
Target Variable: Detection type (Suspicious or Normal traffic)

⚙️ Project Workflow
Data Preprocessing includes removing duplicate records, converting timestamp columns to datetime format, standardizing categorical values, and performing feature engineering such as session duration and average packet size calculation.
Exploratory Data Analysis (EDA) involves analyzing traffic volume distributions, country-wise traffic patterns, detection type distribution, correlation analysis between numerical features, and time-series analysis of web traffic.
Model Training & Evaluation includes anomaly detection using Isolation Forest and classification using Random Forest. Evaluation is performed using accuracy, precision, recall, F1-score, and visual validation of detected anomalies.

🏆 Model Performance Summary
Isolation Forest effectively identified abnormal web traffic sessions based on traffic behavior patterns. Random Forest classifier achieved high accuracy in distinguishing suspicious and normal web interactions, making it the best-performing model for this project.

📈 Visual Results
The project includes visualizations such as bytes_in vs bytes_out distribution, traffic by source country, detection types by country, correlation heatmap, anomaly detection scatter plots, time-series traffic analysis, and network graphs showing source IP to destination IP interactions.

🧾 Files in This Repository
cybersecurity_project.ipynb contains the complete project implementation.
CloudWatch_Traffic_Web_Attack.csv is the dataset used for analysis and modeling.
outputs/images/ stores all generated visualizations.
outputs/code/cybersecurity_project.py contains the Python script version of the project.
outputs/processed_data.csv contains the cleaned and processed dataset.

🧩 Technologies Used
Python 3, Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, NetworkX, and AWS CloudWatch (dataset source).

📚 Future Improvements
Future enhancements include real-time threat detection using streaming data, integration with AWS WAF logs, advanced deep learning models for threat classification, deployment as a web-based security dashboard, and automated alert generation for detected attacks.

👨‍💻 Author
Neeraj Relangi
🎓 Graduate at Andhra University
📧 relangineeraj@gmail.com
