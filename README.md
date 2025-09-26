## Airbnb NYC Listings EDA (2024)

This project performs Exploratory Data Analysis (EDA) on New York Airbnb data to uncover trends and patterns in rental listings. I use libraries like **Pandas, Numpy, Matplotlib, Seabornfor cleaning, visualization, and analysis**.

<img width="1000" height="500" alt="Airbnb-Logo" src="https://github.com/user-attachments/assets/dc92860e-6e56-4697-9d28-0b46c421f763" />


---

## 📌 Project Overview
This project explores Airbnb listing data from New York City using **Pandas, NumPy, Matplotlib, and Seaborn**.  
The aim is to clean, analyze, and visualize the dataset to generate insights that can help both **guests** and **hosts**.  

---

## 🎯 Objectives
- Analyze **room types**, **pricing**, and **availability** across boroughs.  
- Understand **host activity** and identify professional hosting patterns.  
- Detect **outliers** in pricing and availability.  
- Provide **actionable recommendations** for guests and hosts.  

---

## 📂 Dataset
- **Size**: ~20,765 rows × 22 features  
- **Key Columns**:  
  - `id`, `name`, `host_name`  
  - `neighborhood_group`, `neighborhood`  
  - `latitude`, `longitude`  
  - `price`, `room_type`  
  - `reviews_per_month`, `availability_365`  
  - `last_review`  

---

## ⚙️ Workflow

### 1. Data Cleaning
- Handled missing values in `price`, `beds`, `neighborhood`.  
- Converted `last_review` to **datetime**.  
- Removed or capped extreme outliers (`price > $1,500`).  

### 2. Exploratory Data Analysis
- **Room types**: Distribution analysis via bar charts.  
- **Neighborhood groups**: Price comparisons across boroughs.  
- **Availability trends**: Correlation heatmaps and pairplots.  
- **Price distribution**: Histograms and boxplots.  
- **Host behavior**: Listings per host, pricing variation.  

### 3. Visualization Tools
- **Bar charts** for room/neighborhood distribution.  
- **Histograms & Boxplots** for price ranges and outliers.  
- **Heatmaps** for correlation.  
- **Pairplots** for multi-variable relationships.  

---

## 🔑 Key Insights
1. **Manhattan** has the highest average prices, followed by Brooklyn.  
2. **Entire homes/apartments** dominate but cost much more than private rooms.  
3. Outliers exist with prices above **$10,000+**, requiring filtering.  
4. Listings with **high availability** tend to be cheaper and attract more reviews.  
5. Some hosts manage multiple listings → professional hosting behavior.  

---

## 💡 Recommendations
- **For Guests**:  
  - Choose **private rooms in Brooklyn** for affordable stays.  
  - Look for listings with **high availability + good reviews** for a better experience.  

- **For Hosts**:  
  - Adjust **pricing** competitively within boroughs.  
  - Keep listings **highly available** and maintain **positive reviews**.  

---

## 🚀 How to Run
```bash
# Clone the repository
git clone https://github.com/Saswati-18/EDA-New-York-Airbnb-Listings-.git

# Install dependencies
pip install pandas numpy matplotlib seaborn

# Open the notebook
jupyter notebook Airbnb_EDA.ipynb
