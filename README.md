# Analyze company financial health


### ⚠️ The Business Problem: The Growth Paradox
While the enterprise achieved aggressive revenue scaling (expanding from 0.7B to over 2.0B VND), its financial health silently deteriorated. Gross Margin remained stable (11-16%), yet Net Margin collapsed to a critical low of **1.7%**. This wide margin gap revealed massive "hidden costs" leaking through inefficient promotional campaigns, high return rates, and systemic inventory imbalances.

### 🔍 Key Audit Findings & Data Insights
1. **Promotion & Price Erosion Audit:**
   * High-volume percentage discounts accounted for 35.2% of the mix but generated a bottomed net profit of only 2,000 VND/order.
   * Neglected fixed discounts made up only 3.2% of the mix but were **3.5x more profitable** (681,000 VND per 100 orders).
   * The percentage discount trend line showed a steep negative slope (-1.07), risking a drop to absolute break-even if unchecked.
2. **Customer Returns & Workflow Failure Audit:**
   * A total of 510.6M VND in revenue was eroded by product returns.
   * Systemic defects—namely `wrong_size` (34.6%) and `defective` (20.3%)—constituted 73.6% of total return value across all categories.
   * Optimizing the size chart policy to reduce size-related returns to 20% projects a passive recovery of **13.5M VND/day**.
3. **Supply Chain & Capital Efficiency Audit:**
   * Stockouts in high-demand segments (Streetwear/Everyday, Balanced) caused 238.7M VND in lost revenue.
   * The overall 96% fill rate created an **"Average Masking Effect"**, hiding a critical deficit in Hero SKUs that accounted for 81.2% of total lost revenue.
   * At the same time, **40.51B VND in dead capital** was trapped in overstock (1,169 SKUs overstocked for ≥3 consecutive months) due to procurement delays.

### 🛠️ Tech Stack & Architecture
* **Cloud Database:** Supabase (PostgreSQL) 
* **Data Analytics & Modeling:** Python (Pandas, NumPy) for exploratory data analysis, trend calculation, and statistical profiling.

### 📁 Repository Structure
```text
supply-chain-risk-audit/
│
├── EDA.ipynb                       file notebook phân tích và trực quan hóa dữ liệu
│   
├──  
│
├── .gitignore                      <- Prevents uploading large data files or cached directories
├── README.md                       <- Project documentation and business context
