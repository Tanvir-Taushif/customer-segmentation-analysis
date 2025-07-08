# 📊 Customer Segmentation and Pricing Strategy Optimization

This project analyzes a sales dataset to uncover trends in customer behavior across different segments, optimize pricing strategies, and improve overall profitability. The dataset includes order details, customer information, product categories, sales, and shipment data.

---

## 📁 Dataset Overview

The dataset (`dataset.csv`) contains the following key columns:

- **Order_Date, Ship_Date**: Used to calculate lead time
- **Sales**: Revenue per transaction
- **Segment**: Customer group (`Consumer`, `Corporate`, `Home Office`)
- **Category**: Product category (`Furniture`, `Office Supplies`, `Technology`)
- **Region/State**: For geographic analysis
- **Discount**: Estimated from industry benchmarks
- **Profit**: Calculated based on average profit margin per category

---

## ⚙️ Data Processing Steps

- Cleaned and parsed mixed-format dates using logical constraints  
- Calculated **Lead Time** as the difference between `Ship_Date` and `Order_Date`  
- Estimated **Discount** and **Profit** using the following category-based assumptions:

| Category         | Avg. Discount | Avg. Profit Margin |
|------------------|---------------|--------------------|
| Furniture         | 17.39%        | 12.50%             |
| Office Supplies   | 22.15%        | 8.75%              |
| Technology        | 5.20%         | 25.30%             |

---

## 🔍 Key Insights

- 🔻 **Higher discounts did not improve sales** across any customer segment.
- 📉 **Profitability declined** with increased discounts, especially in the Home Office segment.
- 💼 The **Consumer segment** had the highest number of orders and revenue, but the **lowest profit per item**.
- 🧾 The **Home Office segment** generated the **highest profit margin**, suggesting price resilience.


---

## 📷 Visual Insights

### Sales and Profit by Segment

![Sales by Segment](images/1.JPG)

---

### Discount vs Profit Correlation

![Discount vs Profit](images/2.JPG)

---

### Lead Time Distribution

![Lead Time Histogram](images/3.JPG)

---

### Profit Margin by Category and Segment

![Profit by Segment & Category](images/4.JPG)

---

## 💡 Recommendations

1. **Reduce blanket discounts** for low-margin categories like Office Supplies
2. **Apply premium pricing** in Technology where demand is less price-sensitive
3. **Optimize shipping processes** to reduce long lead times in low-performing regions
4. **Target profitable segments** with personalized promotions

---

## 📈 Tools & Technologies

- Python (Pandas, Seaborn, Matplotlib, Plotly)
- Jupyter Notebook
- Data parsing via `dateutil`
- Statistical correlation and group analysis

---

## 📎 How to Run

1. Place `dataset.csv` in the root directory
2. Run `analysis.ipynb` in Jupyter
3. All graphs are automatically generated
4. Images are saved in the `images/` folder for documentation/reporting

---

## 📬 Contact

For questions or collaboration, feel free to reach out!

