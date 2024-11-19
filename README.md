Here’s a well-organized and visually enhanced `README.md` file for the RFM-based customer segmentation project:

---

# 🌟 FLO RFM Customer Segmentation

This project implements **RFM (Recency, Frequency, Monetary)** analysis to segment FLO’s customers based on their purchase behavior. It enables tailored marketing strategies for customer retention and acquisition.

---

## 🚀 Project Overview

### 📝 Purpose
**FLO** aims to optimize its marketing strategies by grouping customers into actionable segments. This project identifies customer behaviors using RFM metrics and assigns them to predefined segments, aiding in decision-making for campaigns and promotions.

### 📊 Dataset
The dataset contains purchase history for **OmniChannel** customers (online and offline) during 2020-2021.

---

## 📂 Dataset Features

| Column Name                     | Description                                            |
|---------------------------------|--------------------------------------------------------|
| `master_id`                     | Unique customer identifier                            |
| `order_channel`                 | Platform used for shopping (e.g., Android, iOS)       |
| `last_order_channel`            | Platform of the most recent purchase                  |
| `first_order_date`              | Date of the first purchase                            |
| `last_order_date`               | Date of the most recent purchase                      |
| `order_num_total_ever_online`   | Total number of online purchases                      |
| `order_num_total_ever_offline`  | Total number of offline purchases                     |
| `customer_value_total_ever_online` | Total spending on online purchases                  |
| `customer_value_total_ever_offline` | Total spending on offline purchases                |
| `interested_in_categories_12`   | Categories purchased in the last 12 months           |

---

## 🔧 Key Features

### 🛠 Tasks

1. **Data Preparation**:  
   - Preprocess data, handle outliers, and engineer new features.  
2. **RFM Metric Calculation**:  
   - Calculate **Recency**, **Frequency**, and **Monetary** values.  
3. **Score Calculation**:  
   - Assign scores to RFM metrics and create **RF** and **RFM Scores**.  
4. **Segmentation**:  
   - Categorize customers into predefined RFM segments based on scores.  
5. **Actionable Insights**:  
   - Extract customer IDs for targeted campaigns.

---

## 📈 Project Workflow

### 1️⃣ Data Preparation
- Aggregate total purchases and spending.  
- Convert date columns into proper datetime format.  
- Analyze distribution of customers across channels and their purchase behaviors.

### 2️⃣ RFM Metrics
- **Recency**: Days since last purchase.  
- **Frequency**: Total number of purchases.  
- **Monetary**: Total spending by the customer.

### 3️⃣ RFM Score Calculation
- Assign scores (1-5) for each RFM metric using quantiles.  
- Combine scores to create **RF_SCORE** and **RFM_SCORE**.

### 4️⃣ Customer Segmentation
- Map RF scores to predefined segments such as `Champions`, `Loyal Customers`, `At Risk`, etc.

---

## 📊 Results

### 🎯 Customer Segments

| Segment               | Description                                  |
|-----------------------|----------------------------------------------|
| `Champions`           | Most valuable and loyal customers.          |
| `Loyal Customers`     | Repeat customers with high frequency.       |
| `At Risk`             | Previously valuable but now inactive.       |
| `Potential Loyalists` | Recent but frequent buyers.                 |
| `Hibernating`         | Low activity and infrequent purchases.      |

### 🛠 Example Use Cases
1. **Targeting New Campaigns**:  
   - Focus on `Champions` and `Loyal Customers` for premium product promotions.  
2. **Retention Strategies**:  
   - Re-engage `At Risk` and `Hibernating` customers with tailored offers.

---

## 🛠 Tools and Libraries

- **Python**  
- **Pandas**  
- **NumPy**  
- **Datetime**  

---

## 🌟 Contribution

Contributions are welcome!  
Feel free to fork this repository, create issues, or submit pull requests for improvements.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).
