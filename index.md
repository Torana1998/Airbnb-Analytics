---
layout: default
title: Airbnb-lytics Project
---

# 📍 Airbnb-lytics — Data-Driven Insights to Enhance Airbnb Occupancy

This project leverages natural language processing (NLP) and machine learning to help **SingStay**, a fictitious short-term rental business, optimise its Airbnb occupancy strategy.

---

## 🎯 Project Objectives

### 🧩 Business Goals Achieved
- **Data Collection and Assessment**: Gathered data on pricing trends, booking patterns, guest feedback, and property features. Benchmarked top-performing competitors to extract replicable strategies.
- **Competitor Analysis**: Identified and analysed successful Airbnb listings in the local market to determine the factors associated with high occupancy.
- **Optimisation Recommendations**: Developed strategies to enhance the company’s property listings.

### 🧪 Technical Goals Achieved 
- Applied text analytics (TF-IDF, word clouds, and n-gram analysis) to extract language used by hosts in highly rated listings.
- Conducted topic modelling (LDA) on listings and reviews to uncover recurring themes.
- Performed sentiment analysis using **TextBlob** and **BERT**.
- Built a **Random Forest** model to predict occupancy, achieving an **R² score of 0.79**.

---

## 📈 Key Business Insights Gained

Insights from predictive modelling and text analysis were grouped into six actionable areas to guide SingStay's occupancy strategy:

- **🏠 Amenities:** Listings with private entrances, security cameras, workspaces, and TVs drive higher occupancy.  
  → *Recommendation:* Standardise these across properties to boost guest appeal.

- **📊 Listing Performance:** Review volume, guest ratings, and host responsiveness are strong occupancy drivers.  
  → *Recommendation:* Encourage post-stay reviews and maintain Superhost service standards.

- **📆 Booking Policies:** Flexibility (8–60 nights) in stay limits is associated with better performance.  
  → *Recommendation:* Re-evaluate booking policies to optimise length-of-stay rules.

- **📝 Review Themes:** Guests value comfort, location, and unique touches (e.g., thematic design, personalised service).  
  → *Recommendation:* Emphasise comfort in listings and explore differentiated experiences.

- **📍 Location:** Fringe areas like Marina South and Tuas show untapped demand despite fewer listings.  
  → *Recommendation:* Expand into these regions and improve transport/accessibility.

- **💰 Pricing Strategy:** Listings priced between $301–$500 and 1-room units show the highest average occupancy.  
  → *Recommendation:* Align pricing strategies to data-backed bands and promote high-performing unit types.

**Future Strategy:**  
Retrain models with new data over time, apply temporal analysis, and explore advanced ML (e.g., XGBoost) for ongoing optimisation.

---

## 📂 Datasets

Data sourced from [Inside Airbnb](http://insideairbnb.com/get-the-data.html) – Singapore listings:

- `listings.csv`: Raw listing data  
- `reviews.csv`: Guest review data  

---

## 🧰 Tools & Technologies

| Category               | Tools & Libraries                                                  |
|------------------------|---------------------------------------------------------------------|
| **Programming**        | Python (`pandas`, `matplotlib`, `seaborn`)                         |
| **Machine Learning**   | `scikit-learn`, `Random Forest`                                    |
| **NLP & Text Analysis**| `TF-IDF`, `n-grams`, `TextBlob`, `BERT`, `Gensim` (LDA), `pyLDAvis` |
| **Environment**        | Google Colab                                                       |

---

## 🗂️ File Descriptions

### 📁 01 - Raw Data

| File Name       | Description                      |
|-----------------|----------------------------------|
| `listings.csv`  | Raw Airbnb listings data         |
| `reviews.csv`   | Raw guest reviews data           |

---

### 📁 02 - Dimensional Data

| File Name               | Description                                             |
|-------------------------|---------------------------------------------------------|
| `dim_listings.csv`      | Structured listing metadata                             |
| `dim_hosts.csv`         | Host profiles with Superhost status, response rate      |
| `dim_reviews.csv`       | Cleaned and tokenised reviews for text analysis         |
| `fact_availability.csv` | Derived occupancy indicators for modelling              |

---

### 📁 03 - Notebooks

| Notebook                           | Purpose                                                                  |
|-----------------------------------|--------------------------------------------------------------------------|
| `1_data_cleaning.ipynb`           | Data transformation and cleansing                                        |
| `2_text_translation_p1.ipynb`     | Part 1 – Translating and tokenising non-English reviews                  |
| `3_text_translation_p2.ipynb`     | Part 2 – Continued processing of translated text                         |
| `4_eda_predictive_modelling.ipynb`| Exploratory analysis and Random Forest modelling                         |
| `5_text_analytics.ipynb`          | TF-IDF analysis, n-gram extraction, word cloud generation                |
| `6_sentiment_analysis.ipynb`      | Sentiment comparison using TextBlob and BERT                             |

---

### 📄 04 - Project Report

| File Name            | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| `Project Report.pdf` | Comprehensive project summary with visualisations and business recommendations |


🔗 [Back to Portfolio](https://torana1998.github.io/)
