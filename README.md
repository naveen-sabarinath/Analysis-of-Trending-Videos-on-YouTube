# YouTube Trending Data Analysis (UK)

This project analyzes UK-based YouTube trending data using data cleaning, exploratory analysis, and machine learning models to understand the factors that influence whether a video trends. It was developed as part of the COMP5721M: Programming for Data Science coursework at the University of Leeds.

## 📊 Project Overview

The project explores over 230,000 entries of trending YouTube videos collected from the YouTube API and Kaggle. The aim is to extract key patterns and attributes that influence a video’s likelihood to trend — with a special focus on view count, likes, category, and upload time.

## 👥 Team Members

- Asish Panda (mm23ap@leeds.ac.uk)  
- Mohamed Imthiyas Abdul Rasheeth (mm23m2ia@leeds.ac.uk)  
- Naveen Sabarinath Babu (mm23nsb@leeds.ac.uk)  
- Roshan . (mm23rt@leeds.ac.uk)

---

## 📁 Dataset

- `GB_youtube_trendingdata.csv`: UK YouTube trending video data (238K+ rows, 16 columns)
- `GB_category_id.json`: Category metadata to decode `categoryId` values

[Dataset Source (Kaggle)](https://doi.org/10.34740/KAGGLE/DSV/7112357)

---

## 🎯 Project Objectives

1. **Visualize** top-trending YouTube genres in the UK.
2. **Identify** keywords in titles/descriptions that increase trending chances.
3. **Examine** the impact of likes, dislikes, and view counts on trending.
4. **Predict** view counts using regression models (Linear & Random Forest).

---

## 🛠️ Tools & Libraries

- Python (pandas, NumPy, seaborn, matplotlib)
- Scikit-learn (Linear Regression, Random Forest Regressor)
- WordCloud
- JSON & CSV parsing
- Jupyter Notebooks

---

## 🔄 Data Processing

- Merged CSV and JSON datasets
- Removed duplicates and nulls
- Extracted useful features (month, hour, category)
- Scaled numerical variables and one-hot encoded categorical features

---

## 📈 Key Analyses

### ✅ Category Trends
- Top trending categories: **Entertainment**, **Sports**, **Gaming**, **Music**, **People & Blogs**
- October had the highest trending activity

### ✅ Title & Tag Keywords
- Word clouds generated for top words in trending videos
- Found most trending titles use 6–8 words
- Category-specific keywords identified

### ✅ Engagement Metrics
- High correlation between **likes**, **comment count**, and **view count**
- Videos published between 2AM–7AM or May–September performed better

---

## 🤖 Predictive Modeling

### 1. **Linear Regression**
- MSE: ~9.7e12  
- R² Score: 0.72  
- Underperformed for very high view counts

### 2. **Random Forest Regression**
- Best R² Score: 0.94 with 20 estimators  
- Outperformed linear regression significantly  
- Better fit for high view counts

---

## 📌 Key Findings

- Videos with strong engagement (likes, comments) are more likely to trend.
- Uploading videos between **2AM–7AM** and during **summer months** increases trending chances.
- Keywords like *“Official”, “Teaser”, “Minecraft”* help boost visibility.
- Random Forest Regression predicts view counts with high accuracy.

---

## 📎 Future Work

- Integrate more countries for global comparison
- Apply classification models to directly predict “Will Trend” (Yes/No)
- Include channel metadata, subscriber counts, and watch time

---

## 📜 License

This project is for academic purposes under the University of Leeds COMP5721M module.

---

## 🙌 Acknowledgements

- Kaggle for the dataset
- YouTube API for metadata inspiration
