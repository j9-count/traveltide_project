# traveltide_project

# TravelTide Customer Segmentation & Rewards Program

## Overview

This repository provides an end-to-end machine learning pipeline to segment customers and design targeted rewards for TravelTide, an online travel platform. The goal is to increase retention, booking frequency, and overall customer value.

---

## Quick Start

1. Open `TravelTide_Segmentation.ipynb` in Google Colab.
2. Set database credentials and parameters in Cell 5.
3. Run all cells sequentially.
4. Download results: `customer_rewards_assignment.csv`, `segment_summary.csv`, and presentation charts.

---


**Project Structure**
```
TravelTide_Segmentation_Project/
├── TravelTide_Segmentation.ipynb
├── customer_rewards_assignment.csv
├── segment_summary.csv
├── traveltide_presentation_chart.png
├── investment_vs_revenue_chart.png
├── requirements.txt
├── README.md
├── executive_summary.md
└── presentation_slides.md
```


---

## Data & Scope

- Analyzed 5,149 customers active Jan–Jul 2023.
- 4 PostgreSQL tables: users, sessions, flights, hotels.
- 573 outliers removed; customers must have 7+ sessions.

---

## Technical Stack

- Python 3.10+, pandas, numpy, scikit-learn, SQLAlchemy
- matplotlib, seaborn, plotly

---

## Methodology

- Cleansing & outlier removal (10% of initial cohort).
- Feature engineering (demographic, behavioral, RFM, travel patterns).
- Unsupervised clustering (K-Means, best model: 3 clusters, silhouette 0.132).
- Automated segment interpretation and rewards assignment.

---

## Results

- **Segments Identified:**
  - High-Value Occasional Travelers (41%) – loyalty rewards
  - Budget Occasional Travelers (50%) – value rewards
  - Low-Value Minimal Engagement (9%) – conversion rewards
- **Reward-eligible:** 5,149 customers (100%)
- **Annual ROI:** Conservative 56%, Optimistic 123%

---

## Deliverables

- `customer_rewards_assignment.csv` – personalized reward assignments
- `segment_summary.csv` – segment counts and stats
- `.png` charts for business presentations
- `executive_summary.md`, `presentation_slides.md`

---

## Customization

- Edit cohort in Cell 5 (`COHORT_START_DATE`, `MIN_SESSIONS`).
- Adjust cluster number in Cell 11.

---

## Limitations

- Moderate segment overlap; quarterly re-segmentation recommended.
- Outlier removal may exclude valuable cases.
- ROI depends on user adoption; actual gains may vary.

---

## Dependencies

- See `requirements.txt`

---

## Contact

For technical or business questions, check notebook outputs or see `executive_summary.md`.

---

**License:** TravelTide  
**Authors:** Jubytra Enzmann, Data Science Team  
**Last Updated:** October 2025
