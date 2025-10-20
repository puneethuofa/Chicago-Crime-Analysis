
# 🕵️‍♂️ Chicago Crime Analysis Dashboard (Excel)

### 📌 Project Overview

The **Chicago Crime Analysis Dashboard** is an interactive Excel-based visualization created to analyze crime patterns across different years, races, and charge categories. Using Chicago’s publicly available crime dataset, the dashboard provides insights into the **number of cases filed**, **charge types**, and **demographic distribution of offenses**, helping policymakers and law enforcement better understand crime trends and enforcement focus areas.

This project demonstrates end-to-end **data preparation, transformation, and visualization** capabilities using **Microsoft Excel**, including pivot tables, charts, and interactive slicers for dynamic exploration.


<img width="937" height="697" alt="image" src="https://github.com/user-attachments/assets/4d963832-02a8-4985-b21b-783ada08e5a4" />
---

## 🎯 Objectives

* To explore and visualize the **distribution of criminal cases** filed across years and categories.
* To identify **major charges** contributing to total crime volume.
* To analyze **crime trends by race, statute, and type** of violation.
* To create an **interactive Excel dashboard** that enables filtering and drill-down analysis.

---

## 🧾 Dataset Description

The dataset contains detailed case-level information about criminal filings in Chicago, including the **charges, dates, and racial distribution** of defendants.

| **Column Name**                                  | **Description**                                             |
| ------------------------------------------------ | ----------------------------------------------------------- |
| `CB_NO`                                          | Case Book Number (Unique case identifier)                   |
| `CASE NUMBER`                                    | Case number associated with the record                      |
| `ARREST DATE`                                    | Date and time of arrest                                     |
| `DATE`                                           | Filing date of the charge                                   |
| `RACE`                                           | Race of the individual (Black, White, Hispanic, etc.)       |
| `CHARGE 1 STATUTE` to `CHARGE 4 STATUTE`         | Legal code references for each charge                       |
| `CHARGE 1 DESCRIPTION` to `CHARGE 4 DESCRIPTION` | Description of the specific charge                          |
| `CHARGE TYPE` and `CLASS`                        | Classification of charges (e.g., Felony, Misdemeanor, etc.) |
| `CHARGES STATUTE / DESCRIPTION`                  | Consolidated charge details for reporting                   |


<img width="2048" height="149" alt="image" src="https://github.com/user-attachments/assets/d82d24fe-e456-47ff-9e67-f76d4cf42ee6" />

---

## ⚙️ Data Preparation

The raw dataset required multiple **data cleaning and transformation** steps before dashboard creation:

1. **Data Cleaning**

   * Standardized date formats across columns (`ARREST DATE`, `DATE`).
   * Removed blank and duplicate rows.
   * Handled inconsistent race labels and missing entries.
   * Created a unified “Charge” field combining multiple charge descriptions.

2. **Feature Engineering**

   * Extracted **Year** from the `DATE` column for trend analysis.
   * Created calculated fields to count **Total Cases Filed** by each statute.
   * Categorized cases by **Charge Type** (A, M, F, etc.) and **Charge Class**.

3. **Data Validation**

   * Cross-verified counts of statutes and cases filed for consistency.
   * Ensured dynamic range updates using Excel tables for scalability.

---

## 📊 Dashboard Components

The Excel dashboard was designed using **Pivot Tables**, **Pivot Charts**, and **Slicers** for user interactivity.
It includes the following visual components:

### 1. **KPI Summary Cards**

* **Total Cases Filed**
* **Cases Filed by Charge 1–4 Statutes**

### 2. **Trend Analysis**

* **Bar Chart (Cases Filed by Year)** – Shows year-wise distribution from 2014–2023.
* **Line Chart (Monthly Case Trend)** – Displays case volume variation across months.

### 3. **Demographic Breakdown**

* **Donut Chart (Crimes by Race)** – Visualizes racial distribution of reported cases.

### 4. **Top Offenses**

* **Horizontal Bar Chart (Top 10 Charges)** – Lists the most common crimes such as:

  * *Issuance of Warrant*
  * *Driving on Suspended License*
  * *Possession of Controlled Substance*
  * *Domestic Battery – Bodily Harm*
  * *Retail Theft*

### 5. **Interactive Filters**

* **Slicers for Year and Race** to allow multi-level filtering.
* **Dynamic charts** automatically update based on slicer selections.

---

## 📈 Key Insights

* The **highest volume of cases** was filed in **2014**, with over **93,000 cases**.
* The **number of filings has declined** consistently after 2019, reaching only **1,700 cases in 2023**.
* **Black individuals** represent the largest proportion of reported cases, followed by **White** and **White Hispanic**.
* The **most common charges** include *Issuance of Warrant*, *Driving on Suspended License*, and *Drug Possession*.
* Crime filings are **more frequent in mid-year months (May–August)**, suggesting possible seasonal trends.

---

## 🧠 Analytical Highlights

| Insight Area          | Observation                                                                                   |
| --------------------- | --------------------------------------------------------------------------------------------- |
| **Temporal Trend**    | Sharp decline in cases post-2020, possibly linked to pandemic-related changes.                |
| **Charge Severity**   | Majority of charges are **Misdemeanors (M)** rather than Felonies (F).                        |
| **Race Distribution** | Crimes are predominantly committed by **Black individuals (≈70%)**, followed by White (≈15%). |
| **Charge Patterns**   | *Domestic Battery* and *Retail Theft* remain recurrent categories over multiple years.        |

---

## 🛠️ Tools & Techniques

| **Tool**                   | **Purpose**                                      |
| -------------------------- | ------------------------------------------------ |
| **Microsoft Excel**        | Primary platform for analysis and visualization  |
| **Pivot Tables**           | Aggregation and filtering of large datasets      |
| **Pivot Charts**           | Visualization of KPIs and categorical breakdowns |
| **Slicers**                | Interactive filtering by year and race           |
| **Conditional Formatting** | Enhanced readability for KPIs                    |

---

## 🧩 Skills Demonstrated

* Data cleaning and preprocessing in Excel
* Dynamic dashboard design
* Trend and distribution analysis
* Visual storytelling using data
* KPI formulation and communication

---

## 📁 Deliverables

* **Excel File:** `Chicago_Crime_Analysis.xlsx`
* **Dashboard Preview:**
  ![Dashboard Preview](./Screenshot_Chicago_Crime_Dashboard.png)

---

## 🧾 Future Improvements

* Automate data refresh with Power Query or Python ETL scripts.
* Incorporate geospatial mapping (heatmaps by ZIP code or district).
* Integrate Power BI for advanced drill-through and predictive analytics.
* Add gender-based segmentation and time-of-day analysis.

---

## 👨‍💻 Author

**Puneeth Vijay Krishna Samarla**
M.S. in Information Science – Machine Learning, University of Arizona
📧 [puneethvks9@email.com](mailto:puneethvks9@email.com)
🔗 [LinkedIn](https://www.linkedin.com/in/puneeth-samarla)




