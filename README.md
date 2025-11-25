# CloudWatch-Cybersecurity-Threat-Analysis
A complete end-to-end cybersecurity analytics project using AWS CloudWatch suspicious web traffic logs. Includes data cleaning, EDA, feature engineering, anomaly detection (IsolationForest), classification (RandomForest), and rich visualizations.

CloudWatch Cybersecurity Threat Analysis
This project analyzes suspicious web traffic captured from AWS CloudWatch to identify potential cyberattacks, anomalies, and malicious request patterns.
It follows a real-world cybersecurity analytics workflow using Python, ML models, and data visualization techniques.
📁 Dataset
The dataset used:
CloudWatch_Traffic_Web_Attack.csv
The file contains:
Suspicious web requests
Source and destination IPs
Protocols
Ports
Bytes transferred
Detection rules
Request timestamps
This data simulates real-world threat monitoring used in SOC (Security Operations Center) environments.
🧹 1. Data Cleaning & Preprocessing
Loaded and inspected CloudWatch threat logs
Converted timestamps (creation_time, end_time)
Standardized country codes & protocols
Converted numeric columns
Removed duplicates & handled missing values
🔍 2. Exploratory Data Analysis
Key insights identified through visualizations:
Top countries generating suspicious traffic
Most-targeted ports
Protocol usage patterns
Bytes in/out distribution
Traffic heatmaps
Charts include:
Histograms
Bar charts
Correlation heatmap
Network graph (src_ip → dst_ip)
⚙️ 3. Feature Engineering
Created advanced derived features:
Session Duration
Average Packet Size
Scaled Traffic Metrics
🤖 4. Machine Learning Models
Anomaly Detection — IsolationForest
Identified suspicious vs normal traffic using:
bytes_in, bytes_out, session_duration, avg_packet_size.
Classification — RandomForest
Binary classification using detection rules:
Labeled malicious vs normal records
Achieved strong classification performance
📊 5. Visual Outputs
Includes:
Anomaly scatter plots
Heatmaps
Country attack maps
Protocol/port analysis
Time-based traffic patterns
📂 Project Deliverables
Google Colab notebook (.ipynb)
PowerPoint presentation (.pptx)
Detailed workflow document (.docx)
LinkedIn post visuals (metallic UI-styled PNG)
All charts exported
📌 Skills Used
Python
Pandas, NumPy
Matplotlib
IsolationForest, RandomForest
Feature Engineering
EDA
Cybersecurity Analytics
CloudWatch log analysis
🚀 About This Project
This project is part of the Unified Mentor Cybersecurity & ML Program and simulates real-world threat detection workflows used by security analysts and ML engineers.
