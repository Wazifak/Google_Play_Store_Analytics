# Google Play Store Review Analytics

## 📌 Project Overview
This project analyzes Google Play Store app data to uncover insights on installs, ratings, categories, and trends.  
It includes data cleaning, transformation, and multiple visualization tasks to build an interactive analytics dashboard.

## 📊 Dataset
- **Source**: Google Play Store dataset (apps + global information).
- **Files**:
  - `apps.csv` → Main app-level data
  - `global.csv` → Location-based installs by app
- **Key Columns**:
  - App, Category, Rating, Reviews, Installs, Size, Last Updated, Country (from global_df)

## 🧹 Data Cleaning
1. Removed duplicates and missing values
2. Cleaned `Installs` column (removed "+" and "," → numeric)
3. Converted `Size` to MB
4. Parsed `Last Updated` into datetime and extracted Month/Year
5. Created `Installs_Clean` for numeric analysis

## ✅ Tasks Implemented
### Task 1: Bar chart (Top 10 categories by Avg Rating & Reviews) — Available 3–5 PM IST
- Filter apps with Rating ≥ 4.0, Size ≥ 10MB, Last Updated = January
- Dual-axis bar chart for Avg Rating & Total Reviews

### Task 2: Choropleth map (Installs by Category & Country) — Available 6–8 PM IST
- Excluded categories starting with A, C, G, S
- Top 5 categories selected by installs
- Choropleth shows installs distribution by Country

### Task 3: Dual-axis Chart (Free vs Paid Installs & Revenue)
- Separate Free vs Paid apps
- Bar = Installs, Line = Revenue
- Clear labels on both y-axes

### Task 4: Time Series (Monthly Installs Growth)
- Line chart of installs over time
- Highlight months with >20% growth

### Task 5: Bubble Chart (Category Performance)
- X = Reviews, Y = Rating, Bubble size = Installs
- Highlight “Game” category in pink
- Hover tooltip shows app details

### Task 6: Stacked Area Chart (Cumulative Installs) — Available 4–6 PM IST
- Cumulative installs per category by month
- Categories translated into multiple languages
- Growth >25% emphasized with styling

## 🔖 Author
- **Wazifa Kapdi**  
Data Science Intern | Google Play Store Review Analytics Project
