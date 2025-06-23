# Retail Customer Segmentation Using RFM Analysis

## Project Overview

This project performs **Customer Segmentation** on retail transaction data using **RFM (Recency, Frequency, Monetary)** analysis. The goal is to identify distinct customer groups based on their purchase behavior to support targeted marketing and improve customer retention strategies.

The analysis uses a real-world online retail dataset and demonstrates how to:

- Calculate RFM metrics for each customer  
- Score and segment customers based on their recency, purchase frequency, and monetary value  
- Visualize RFM score distributions  
- Identify best customers and potential segments for personalized engagement  

---

## Dataset

- The dataset contains transaction records of an online retail store.  
- Key columns include: `Customer ID`, `InvoiceDate`, `Invoice`, `Quantity`, and `Price`.

---

## Project Structure

- `notebooks/` — Jupyter notebooks containing data exploration, RFM calculation, scoring, and visualization  
- `data/` — Raw and processed dataset files  
- `rfm_scores.csv` — Output file with calculated RFM scores and segments  

---

## Key Steps

1. **Data Cleaning & Preprocessing:**  
   Convert dates, calculate total price per transaction, handle missing values.

2. **RFM Calculation:**  
   Aggregate data per customer to calculate recency (days since last purchase), frequency (number of purchases), and monetary value (total spending).

3. **RFM Scoring:**  
   Assign scores (1-5) for each RFM metric based on quintiles, where a higher score indicates better customer value.

4. **Segmentation & Visualization:**  
   Combine scores to form customer segments and visualize the distribution of RFM scores.

---

## How to Run

1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/retail-customer-segmentation.git
   cd retail-customer-segmentation
2. Setup Python ENV:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows use `venv\Scripts\activate`
   pip install -r requirements.txt

## Libraries Used

- pandas
- matplotlib
- seaborn

## Future Work
- Implement clustering algorithms (e.g., K-Means) for more granular segmentation
- Integrate predictive modeling for customer churn and lifetime value
- Develop dashboards for interactive exploration

## License
Free to use. :)
