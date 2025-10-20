<!-- README.md -->

<h1 align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Montserrat&size=28&duration=3500&color=E50914&center=true&vCenter=true&width=500&lines=🎬+Netflix+Analysis+Project;📊+Data+Exploration+%26+Visualization;🚀+Python+%7C+Pandas+%7C+Seaborn+%7C+Matplotlib" alt="Typing Animation">
</h1>

---

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9+-blue?logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Library-Pandas%20%7C%20NumPy%20%7C%20Matplotlib%20%7C%20Seaborn-orange?logo=python">
  <img src="https://img.shields.io/badge/Data%20Source-Netflix%20Dataset-red?logo=netflix">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=flat">
</p>

---

## 🧠 **Project Overview**

This project dives deep into the **Netflix dataset**, exploring its movies and TV shows to uncover meaningful trends in content type, rating, country distribution, and release patterns.

It focuses on:
- Data cleaning and preprocessing  
- Exploratory data analysis (EDA)  
- Visualization of trends using **Matplotlib** and **Seaborn**

---

## 🧩 **Tech Stack**

| Tool | Description |
|------|--------------|
| **Python** | Core programming language |
| **Pandas** | Data manipulation and analysis |
| **NumPy** | Numerical computation |
| **Matplotlib / Seaborn** | Visualization and insights |
| **Jupyter Notebook** | Interactive data analysis |

---

## 📂 **Dataset Overview**

| Feature | Description |
|----------|--------------|
| `Show_Id` | Unique ID for each show |
| `Category` | Movie or TV Show |
| `Title` | Name of the content |
| `Director`, `Cast`, `Country` | Metadata |
| `Release_Date` | Date of release |
| `Rating` | Content rating (TV-MA, R, PG, etc.) |
| `Duration` | Movie duration or TV seasons |
| `Type` | Genre information |
| `Description` | Short summary |

**Dataset Shape:** `(7789, 11)` → after cleaning → `(4811, 11)`

---

## 🧹 **Data Cleaning Steps**

1. **Handled Missing Values** – Dropped rows with nulls in key columns.  
2. **Converted Dates** – Parsed `Release_Date` into datetime format.  
3. **Extracted Numeric Duration** – Created `Duration_final` for analysis.  
4. **Standardized Columns** – Ensured data uniformity.

---

## 📊 **Data Visualization**

Here are some of the visual insights extracted:

### 🎞️ Category Distribution by Rating
```python
sns.countplot(x=df['Category'], hue=df['Rating'])
```
Shows how Movies dominate across ratings like TV-MA, TV-14, etc.

### 🌍 Top 10 Countries Producing Content
```python
sns.countplot(y='Country', data=df[df['Country'].isin(top_countries)], order=top_countries)
```
United States and India lead by a large margin in Netflix productions.

### ⏱️ Average Duration by Genre

Pie chart visualization of top genres by average movie duration.

### 📈 Yearly Trend of Releases
```python
sns.lineplot(data=yearly, x='Year', y='Count', hue='Type', marker='o', palette='flare')
```
A beautiful line graph showing the growth of movies vs TV shows over time.

### 🔥 Rating vs Duration Heatmap
```python
sns.heatmap(heat_data, cmap='YlGnBu')
```
Visualizes correlation between content ratings and duration.

## 📸 Sample Visuals
## 🚀 Key Insights

 - 🎬 Movies dominate Netflix’s catalog (over 90% of titles).

 - 🌍 US & India contribute most to Netflix’s global library.

 - ⏳ Average movie duration ≈ 93 minutes.

 - 📅 Significant growth in releases from 2015–2020.

 - 🔞 Majority of content rated TV-MA (Mature Audience).

## 🧭 Future Scope

 - Integrate interactive dashboards (Plotly / Streamlit).

 - Add recommendation engine using ML.

 - Automate data updates via API or web scraping.

   
## 🧑‍💻 Author

Pushkar Khattri
Frontend Engineer | Data & AI Enthusiast

<p align="left"> <a href="https://github.com/PushkarKhattri"> 
  <img src="https://img.shields.io/badge/GitHub-PushkarKhattri-black?logo=github" /> 
</a> <a href="mailto:pushkarkhattri@gmail.com"> 
  <img src="https://img.shields.io/badge/Email-Contact-blue?logo=gmail" /> 
</a> <a href="https://www.linkedin.com/in/pushkarkhattri/"> 
  <img src="https://img.shields.io/badge/LinkedIn-Connect-informational?logo=linkedin" />
</a> </p>

<h3 align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Poppins&size=22&duration=3500&color=E50914&center=true&vCenter=true&width=500&lines=Thanks+for+Reading+❤️;Don't+forget+to+⭐+the+repository!">
</h3> 


