# Retail-Store-Shelf-Placement-Optimization-association_rule
Leverages retail transaction data and association rules to design optimal shelf layouts, streamline product adjacencies, and increase customer footfall and basket size.

# 🏬 Retail Store: Shelf Placement Optimization & Market Basket Analytics

## 1. Business Problem

### 1.1. What is the business objective?
* **Optimizing Product Adjacencies:** Analyze transactional records from a retail store in India to discover local consumer buying patterns and product affinities.
* **Store Layout & Shelf Placement:** Provide store managers with data-driven rules on how to arrange products on shelves strategically to improve buying behavior, encourage impulse purchases, and increase customer footfall and basket size.

### 1.2. Are there any constraints?
* **Physical Store Layout Limits:** Working within the physical constraints of aisle dimensions, shelf capacity, and product grouping logic.
* **Algorithm Parameter Tuning:** Balancing support and confidence thresholds to filter out noise and extract high-lift, actionable shelf-stocking rules.

---

## 2. Data Dictionary (`transaction_retail.csv`)

| Feature Name | Data Type | Description |
| :--- | :--- | :--- |
| **Transaction_ID / Basket_ID** | Integer / String | Unique identifier for each customer checkout transaction at the retail store. |
| **Product_Item / SKU** | Categorical | Names or codes of the retail products purchased together in a basket. |

---

## 3. Data Pre-processing

### 3.1. Data Cleaning & Feature Engineering
* **Data Transformation:** Processed raw transactional logs into structured one-hot encoded boolean matrices representing store baskets.
* **Sanitization:** Checked for missing values, normalized product nomenclature, and removed erroneous entries to ensure data integrity.

---

## 4. Model Building

### 4.1. Application of Apriori Algorithm
* Implemented the Apriori algorithm via Python libraries (e.g., `mlxtend`) to uncover frequent itemsets that satisfy minimum support parameters.
* Evaluated association rules using **Confidence** and **Lift** to identify strong product co-purchases.

### 4.2. Frequent Itemsets & Rule Visualization
* Generated frequent itemsets and visualized association rules using scatter plots and network graphs to map store product adjacencies clearly.

### 4.3. Work on Codes
* The complete source code implementation is stored in the `transaction_retail.py` file.

---

## 5. Deployment

### 5.1. Deploy Solutions
* The resulting placement rules can be compiled into a visual merchandising guideline manual or layout optimization dashboard for store managers.

---

## 6. Business Impact & Benefits
* **Optimized Shelf Arrangement:** Placing complementary items adjacent to each other makes shopping intuitive and boosts cross-selling.
* **Increased Footfall & Basket Size:** Enhances the overall in-store shopping experience, leading to higher customer retention, larger transaction sizes, and increased revenue.
