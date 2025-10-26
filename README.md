Customer Segmentation and Product Recommendation System
by Poojitha Gollapudi

📊 Project Overview
This project implements a comprehensive customer segmentation and product recommendation system using transaction data to identify distinct customer groups and generate personalized product recommendations. The system uses RFM analysis and K-means clustering to segment customers based on their purchasing behavior.

🎯 Business Problem
Understanding customer behavior is crucial for targeted marketing, personalized recommendations, and improving customer retention. This project helps businesses:

Identify different customer segments

Understand purchasing patterns

Generate personalized product recommendations

Optimize marketing strategies

Insight: This visualization clearly demonstrates the spending patterns across different clusters, showing Cluster 1 as the highest spending group, followed by Cluster 2 and Cluster 0.

📁 Project Structure
text
Customer_Segmentation_Project/
├── Customer_Segmentation_Project.ipynb
├── sample_transactions.csv
├── WhatsApp Image 2025-10-26 at 15.45.42_90d15dbc.jpg
├── WhatsApp Image 2025-10-26 at 15.45.42_cabcdd10.jpg
└── README.md
🛠 Technologies Used
Python 3.12.0

pandas - Data manipulation and analysis

numpy - Numerical computations

scikit-learn - Machine learning (K-means clustering)

matplotlib & seaborn - Data visualization

datetime - Date handling for recency analysis

📈 Methodology
1. Data Processing & Cleaning
Load transaction data from CSV

Handle missing values:

Drop rows with missing CustomerID or ProductID

Fill missing PurchaseAmount with 0

Fill missing Category with "Unknown"

Ensure correct data types for analysis

2. Feature Engineering (RFM Analysis)
Recency: Days since last purchase

Frequency: Number of purchases per customer

Monetary: Total and average spending

Category Preference: Most purchased product category

3. Customer Segmentation
K-means Clustering with 3 clusters

Features used: Total_Spent, PurchaseCount, AvgPurchaseAmount, RecencyDays

StandardScaler for feature normalization

4. Recommendation System
Three recommendation strategies implemented:

Total Amount-Based: Categories with highest spending

Frequency-Based: Most frequently purchased categories

Hybrid Approach: Combined score of amount and frequency

📊 Results
Customer Segments Identified:
Cluster 0: Low to moderate spenders, mixed category preferences

Cluster 1: High-value customers, electronics-focused

Cluster 2: Moderate spenders with multiple purchases, electronics and fashion

Key Insights:
Electronics is the most profitable category across segments

Cluster 1 represents high-value customers needing premium targeting

Cluster 0 shows potential for cross-selling opportunities

Visual analysis confirms clear spending differentiation between clusters

🚀 How to Run
Prerequisites
bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
Execution
Clone or download the project files

Ensure sample_transactions.csv is in the same directory

Open Jupyter Notebook:

bash
jupyter notebook Customer_Segmentation_Project.ipynb
Run all cells sequentially

Input Data Format
The system expects a CSV file with the following columns:

CustomerID: Unique customer identifier

ProductID: Unique product identifier

Category: Product category

PurchaseAmount: Transaction amount

PurchaseDate: Date of purchase (YYYY-MM-DD)

💡 Business Applications
Marketing Strategies
Cluster 1: Premium offers, loyalty programs

Cluster 0: Cross-selling, frequency incentives

Cluster 2: Bundle deals, category expansion

Personalization
Tailored product recommendations

Customized email campaigns

Segment-specific promotions

Customer Retention
Identify at-risk customers (high recency)

Reactivation campaigns

Lifetime value optimization

🔮 Future Enhancements
Incorporate more customer demographics

Implement real-time recommendation engine

Add time-series analysis for trend prediction

Develop dashboard for business users

Integrate with e-commerce platforms

📋 Dependencies
python
pandas>=1.5.0
numpy>=1.21.0
matplotlib>=3.5.0
seaborn>=0.11.0
scikit-learn>=1.0.0
jupyter>=1.0.0
👤 Author
Poojitha Gollapudi
Data Science and Machine Learning Enthusiast

📄 License
This project is open source and available under the MIT License.

Note: This project uses synthetic transaction data for demonstration purposes. Replace sample_transactions.csv with your actual transaction data for real-world applications.
