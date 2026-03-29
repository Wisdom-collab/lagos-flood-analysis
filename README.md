# 🌊 Lagos Flood Risk Analysis (2010–2024)

## 📌 Project Overview
Flooding remains one of the most critical urban challenges in Lagos, Nigeria, driven by intense rainfall, poor drainage systems, and rapid urbanization.  

This project analyzes **historical weather data (2010–2024)** to:
- Identify key weather variables influencing flood risks  
- Detect seasonal and yearly flooding patterns  
- Build an interactive dashboard for insights and decision-making  

The analysis combines **data cleaning (Google Sheets)** and **interactive visualization (Power BI)** to generate actionable insights for urban resilience.

---

## 🎯 Objectives
- Analyze rainfall trends over time  
- Identify **flood-prone months and periods**  
- Examine relationships between:
  - Rainfall (`Precip`)
  - Rainfall probability (`Preciprob`)
  - Sea-level pressure (`SealevelPressure`)  
- Provide **data-driven recommendations** for flood mitigation  

---

## 🗂️ Dataset Description
- Historical weather dataset for Lagos (2010–2024)  
- Total observations: **3,558 records**

### Key Variables
- `Date`  
- `Precip` (Rainfall amount)  
- `Preciprob` (Rain probability)  
- `SealevelPressure`  
- `Season`  
- `Precitype`  

📥 **Dataset Access**  
[[Download Dataset](https://docs.google.com/spreadsheets/d/1uuPbvKzWqkbgHZ7E2wkn1UX5Jo2kJa26/edit?usp=sharing&ouid=117932305957074909801&rtpof=true&sd=true)]

---

## 🧹 Data Preparation (Google Sheets)

### Data Cleaning
- Removed duplicates (Date + Location)
- Standardized date formats
<img width="1087" height="493" alt="Flood Risk Dataset" src="https://github.com/user-attachments/assets/c70af7bc-557c-462d-a760-c0328fc6ea4e" />


### Handling Missing Values
- `Precitype`:
  - `"None"` if rainfall = 0  
  - `"Rain"` if rainfall > 0  
  - `"Unknown"` where unclear  

### Feature Engineering
Created key variables:

#### Rainfall Intensity
- No Rain (0 mm)  
- Light (≤2 mm)  
- Moderate (2–10 mm)  
- Heavy (10–50 mm)  
- Extreme (>50 mm)  

#### Flood Risk Flag
Defined using:
- High rainfall levels  
- Rainfall probability  
- Low sea-level pressure  

---

## 📊 Dashboard Overview (Power BI)
[[Interact with the dashboard here](https://drive.google.com/file/d/1eDZCuq-Ej3sszodF_xXdpu-vVTwH_STE/view?usp=sharing)]
### 🖼️ Dashboard Preview
![Flood Risk Dashboard](https://github.com/user-attachments/assets/779277e0-3d9f-4731-892f-5e656c101857)

---

## 📈 Key Metrics (KPIs)
- **Average Rainfall/Year:** 4.81 mm  
- **High-Risk Days/Year:** 604 days  
- **Flood Risk Probability:** 52.50%  

These indicators show that **flood risk is both frequent and significant** in Lagos.

---

## 🔍 Dashboard Analysis & Insights

### 1. 📉 Annual Rainfall Trends
- Rainfall peaked around **2011–2012 (~3.9K mm)**  
- A steady decline occurred until **2019 (~1.1K mm)**  
- Slight recovery observed from **2020–2023 (~1.6K–1.9K mm)**  
- Sharp drop in **2024 (~0.2K mm)** (likely incomplete year)

👉 **Insight:** Flood risk is not only about total rainfall but also **intensity and distribution over time**.

---

### 2. 📅 Monthly Rainfall Seasonality
- Peak rainfall occurs in:
  - **June, July, September**
- Low rainfall months:
  - **January, February, December**

👉 **Insight:** Lagos exhibits a **strong seasonal rainfall pattern**, aligning with the **rainy season (April–October)**.

---

### 3. ⚠️ Flood-Prone Months Across Years
- Highest risk months:
  - **March (~105 occurrences)**
  - **April (~91)**
  - **February (~72)**
- Risk gradually declines toward later months

👉 **Insight:** Flood risks **start earlier than peak rainfall months**, suggesting:
- Drainage inefficiencies  
- Early-season storms triggering floods  

---

### 4. 🔗 Correlation: Rainfall vs Probability vs Pressure
- Rainfall probability trends closely follow rainfall patterns  
- Sea-level pressure shows an **inverse relationship**:
  - Lower pressure → higher rainfall likelihood  

👉 **Insight:**  
Flood conditions are most likely when:
- Rainfall probability is high  
- Sea-level pressure is low  

---

### 5. 📊 Scatter Analysis (Rainfall vs Pressure)
- High-risk points cluster where:
  - Rainfall is high  
  - Pressure is relatively low  

👉 **Insight:** Confirms that **combined atmospheric conditions** drive flood risk, not just rainfall alone.

---

## ⚠️ Limitations
- No direct flood event records (only weather indicators)  
- Missing values in `Precitype`  
- Limited spatial coverage (few stations)  
- Binary rainfall probability (0 or 100)  

---

## 💡 Recommendations

### Short-Term (Mitigation)
- Improve drainage systems before peak months (March–July)  
- Deploy early warning systems using rainfall thresholds  
- Monitor high-risk conditions (low pressure + high rainfall probability)  

### Long-Term (Adaptation)
- Invest in flood-resilient infrastructure  
- Improve urban planning and zoning policies  
- Adopt green infrastructure (permeable surfaces, drainage expansion)  

---

## 🛠️ Tools & Technologies
- **Google Sheets** – Data cleaning  
- **Power BI** – Dashboard & visualization  
- **Pivot Tables & Formulas** – Analysis  

---

## 📁 Project Structure

📦 lagos-flood-analysis
 ┣ 📂 data
 ┃ ┗ cleaned_flood_data.csv
 ┣ 📂 images
 ┃ ┗ dashboard_screenshots.png
 ┣ 📂 dashboard
 ┃ ┗ flood_dashboard.pbix
 ┣ 📜 README.md


---

## 🚀 How to Use
1. Download the dataset  
2. Open the Power BI file (`.pbix`)  
3. Interact with filters (Month, Year, Season)  
4. Explore trends and flood risk patterns  

---

## 📬 Contact
**Wisdom Daberechukwu Nwachukwu**  
📧 ndwisdom96@gmail.com  
🔗 https://www.linkedin.com/in/wisdom-nwachukwu-651522228  

---

## ⭐ Acknowledgements
This project demonstrates the application of data analytics in addressing **urban flooding and climate risk challenges**.

---

## ⭐ If you found this useful
Give this project a ⭐ and feel free to fork or contribute!
