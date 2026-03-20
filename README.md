
# Interactive Spotify Top 50 Analytics Dashboard using Power BI

## 📊 Project Overview

This project focuses on analyzing Spotify’s **Top 50 songs dataset** and transforming raw data into an **interactive Power BI dashboard**.

The dashboard helps stakeholders such as music analysts, playlist managers, and marketing teams gain insights into:

* Song performance
* Artist popularity
* Music trends over time
* Content characteristics (Explicit vs Non-Explicit)

---

## 🎯 Objectives

* Provide a centralized view of key KPIs
* Analyze trends in song popularity
* Compare artist and song performance
* Enable data-driven decision-making

---

## 📁 Dataset

* Source: Spotify Top 50 Dataset (CSV format)
* Contains:

  * Song Name
  * Artist
  * Popularity
  * Duration
  * Album Type
  * Release Date
  * Explicit Flag
  * Position (Ranking)

---

## ⚙️ Tools & Technologies Used

* **Power BI** → Data visualization
* **DAX (Data Analysis Expressions)** → KPI calculations
* **Power Query** → Data cleaning & transformation
* **Microsoft Excel / CSV** → Data source

---

## 📊 Dashboard Features

### 🔹 Overview Page

* Total Songs, Distinct Artists, Avg Popularity, Avg Duration
* Explicit vs Non-Explicit comparison
* Album Type distribution
* Yearly & Monthly trend analysis
* Top Songs & Top Artists

---

### 🔹 Artist Analysis Page

* Top Artists by popularity
* Songs per artist
* Tracks per album comparison
* Artist-level drill-down insights

---

### 🔹 Songs Analysis Page

* Top Songs ranking
* Song distribution by album type
* Detailed table with:

  * Song name
  * Release date
  * Popularity
  * Duration
  * Position

---

## 🧠 Key DAX Measures

Some important measures used:

```DAX
Total Songs = COUNTROWS('Top-50-world')

Distinct Artists = DISTINCTCOUNT('Top-50-world'[artist])

Avg Popularity = AVERAGE('Top-50-world'[popularity])

Explicit Songs = 
CALCULATE(
    COUNTROWS('Top-50-world'),
    'Top-50-world'[is_explicit] = TRUE()
)

Pct Explicit Songs = 
DIVIDE([Explicit Songs], [Total Songs], 0)
```

---

## 📈 Insights Gained

* Identified top-performing songs and artists
* Observed trends in popularity over time
* Compared explicit vs non-explicit song performance
* Analyzed distribution of songs by album type

---

## 🖼️ Dashboard Preview

👉 *<img width="1246" height="710" alt="Screenshot 2026-03-20 173100" src="https://github.com/user-attachments/assets/454bcbc9-6f99-42b4-ac68-a686079e554a" />



```
![Dashboard Screenshot](images/dashboard.png)
```

---

## 🚀 How to Use

1. Download the `.pbix` file from this repository
2. Open in **Power BI Desktop**
3. Explore the dashboard using filters and visuals

---

## 🔮 Future Enhancements

* Integration with Spotify API (real-time data)
* Predictive analytics for hit songs
* Recommendation system
* Advanced visualizations and AI insights

---

## 📚 References

* Spotify Dataset (Kaggle / Open Source)
* Microsoft Power BI Documentation
* DAX Documentation

---

## 👤 Author

**Yogesh Patil **

* GitHub: https://github.com/yogesh-patil2003/
* LinkedIn: *(https://www.linkedin.com/in/yogeshpatil2003/)*

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!

