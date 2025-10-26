# 🛒 Retail Data Preprocessing & Visualization (Week 1 Assignment)

## 📘 Project Overview
This project is part of **Apex FDP – AI Assignment Week 1**.  
It focuses on **data preprocessing** and **visualization** using a retail transaction dataset.

A retail chain wants to analyze customer purchase behavior, understand city-wise sales, and improve decision-making through clean, structured data insights.

---

## 📂 Dataset
**File:** `Retail_Transactions_2000.csv`  
Each row represents a transaction.

### Columns:
- `TransactionID` – Unique transaction ID  
- `CustomerID` – Unique customer ID  
- `Gender` – Male/Female/Other  
- `Age` – Age of customer  
- `City` – City where purchase occurred  
- `ProductCategory` – Product type (Electronics, Fashion, etc.)  
- `Quantity` – Units purchased  
- `Price` – Price per unit (₹)  
- `TotalAmount` – Quantity × Price  
- `PurchaseDate` – Date of purchase  
- `PaymentMode` – Cash, Card, UPI, Wallet  

---

## 🧹 Part A: Data Preprocessing

### Tasks Performed:
1. **Data Inspection**
   - Loaded dataset using `pandas`
   - Checked for missing values, duplicates, and structure

2. **Handling Missing Data**
   - Replaced missing `Age` with median
   - Replaced missing `City` with most frequent city
   - Dropped rows with missing `TransactionID` or `ProductCategory`

3. **Data Cleaning**
   - Removed duplicate rows  
   - Standardized categorical values (e.g., `m`, `MALE` → `Male`)  
   - Removed invalid (negative/zero) `Quantity` or `Price`

4. **Feature Engineering**
   - Derived `TotalAmount` = `Quantity × Price`  
   - Extracted `Month` and `DayOfWeek` from `PurchaseDate`  
   - Created `AgeGroup` (18–25, 26–40, 41–60, 60+)

5. **Final Verification**
   - Ensured no missing or invalid data  
   - Saved cleaned dataset as `Retail_Cleaned.csv`

---

## 📊 Part B: Data Visualization

### Insights Visualized:
| Category | Visualization | Description |
|-----------|----------------|--------------|
| Customer Demographics | Histogram, Pie Charts | Age & Gender distribution, Top 10 cities |
| Sales Insights | Bar & Line Charts | Sales by product category and month |
| Payment Analysis | Pie Chart | Mode of payment usage |
| Advanced Insights | Bar & Heatmap | Avg spend by age group, city revenue, product vs payment mode |

All plots were created using **Matplotlib** and **Seaborn**.

## 1. Customer Demographics
<img width="544" height="396" alt="image" src="https://github.com/user-attachments/assets/1f82b3aa-7282-4a1d-9e7e-35aeff3ecfe4" />
<img width="360" height="348" alt="image" src="https://github.com/user-attachments/assets/457ffacb-42f0-409e-b20b-eaefc65e5a37" />
<img width="678" height="464" alt="image" src="https://github.com/user-attachments/assets/3c07944c-04b4-4cf0-a428-e7c9750d77b5" />

## 2. Sales Insights
<img width="695" height="456" alt="image" src="https://github.com/user-attachments/assets/1189ced7-d2d5-4a3b-8989-471906a7fadb" />

<img width="703" height="396" alt="image" src="https://github.com/user-attachments/assets/b88ad3ac-9645-4567-81dd-798bd66598aa" />

<img width="328" height="348" alt="image" src="https://github.com/user-attachments/assets/c7b5d400-8381-4650-96fd-08c7b0e6989f" />

##  3. Advanced Insights
<img width="552" height="421" alt="image" src="https://github.com/user-attachments/assets/0befbb14-5f80-4a2d-8376-6fe8c12a6c14" />

<img width="703" height="464" alt="image" src="https://github.com/user-attachments/assets/924fd9ef-7dad-411a-8ec5-7a739e26255c" />

<img width="705" height="473" alt="image" src="https://github.com/user-attachments/assets/5699f803-fd6a-4c75-bf08-fdb092b325dd" />


## 💻 How to Run

### 1️⃣ Install Requirements
```bash
pip install pandas matplotlib seaborn
