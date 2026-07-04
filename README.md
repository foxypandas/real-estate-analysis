# 🏠 Real Estate Market Analysis: St. Petersburg

**[EN](README.md) | [RU](README.ru.md)**

Exploratory data analysis of apartment listings (Yandex Real Estate archive): what drives housing prices in St. Petersburg and its suburbs. Bilingual project — full analysis available in English and Russian.

**Key findings:** apartment price is driven primarily by **total area** and **location** — median price 4.65M ₽; half of all apartments sell within **95 days**; publication day and month have no meaningful effect on price.

## 📋 Task

The dataset is an archive of apartment listings for St. Petersburg and nearby settlements. The goal is to identify the parameters that determine market value — groundwork for an automated system that flags anomalies and fraudulent listings.

## 📊 Data

23,699 listings (23,613 after cleaning) listings with two types of features: user-submitted (price, area, rooms, floor, ceiling height) and map-derived (distances to city center, airport, parks and ponds). 

Preprocessing: missing values filled by feature type (medians for numeric, explicit categories for strings), implicit duplicates in settlement names unified, data types converted, outliers filtered by quantiles and IQR.

**Engineered features:** price per m², publication day of week / month / year, floor type (first / last / other), distance to city center in km.

## 🔍 Key Findings

**Price factors.** Total area is the strongest price driver; living area, kitchen area and number of rooms follow (living area correlates with total area at 0.88, so their effects overlap). Price per m² rises with total area (correlation 0.66) — larger apartments are more expensive per meter as well. Balconies, publication day and month show no meaningful effect.

<![Price vs total area](images/price_vs_total_area.png)

**Location.** Prices peak in the city center (0–5 km) and stabilize at 5–25 km. Suburban resort areas (Lisy Nos, Zelenogorsk) show elevated price per m² despite the distance — nature premium at work.

![Price vs distance to center](images/price_vs_distance.png) 

**Market dynamics.** Median time on market — 95 days (mean 168 days, skewed by long-tail listings). Sales within 30 days can be considered fast; listings over 100 days warrant a closer look — potential overpricing or property issues.

## 🛠 Stack

`Python` · `pandas` · `NumPy` · `Matplotlib` · `Seaborn` · `Jupyter`

## 🚀 How to Run

```bash
git clone https://github.com/foxypandas/real-estate-analysis.git
cd real-estate-analysis
pip install -r requirements.txt
jupyter notebook notebooks/real_estate_eda_en.ipynb
```

The dataset is not included in the repository. 

## 📁 Project Structure

```
├── notebooks/     # analysis notebooks (EN and RU versions)
├── images/        # charts and visualizations
└── requirements.txt
```
