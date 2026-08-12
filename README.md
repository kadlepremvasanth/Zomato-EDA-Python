# Zomato Restaurant Data Analysis & Visualization using Python

##  Project Overview
Zomato is one of India's leading food delivery platforms, with an average of 17.5 million monthly transacting customers and 226,000+ active restaurant partners. This project analyzes a Zomato restaurant dataset to uncover customer ordering patterns, restaurant performance, and rating trends using Python-based Exploratory Data Analysis (EDA) and data visualization.

##  Objective
As a data professional working on Zomato's dataset, the goal is to explore the data and answer key business questions that can help improve customer experience and drive targeted offers/promotions.

##  Business Questions Answered
1. What type of restaurant do the majority of customers order from?
2. How many votes has each type of restaurant received from customers?
3. What are the ratings that the majority of restaurants have received?
4. What is the average spending of couples who order food online?
5. Which mode (online or offline) has received the maximum rating?
6. Which type of restaurant received more offline orders, so Zomato can target them with offers?

##  Dataset
- **Rows:** 148
- **Columns:** 7
- **Features:**
  - `name` — Restaurant name
  - `online_order` — Whether online ordering is available (Yes/No)
  - `book_table` — Whether table booking is available (Yes/No)
  - `rate` — Restaurant rating (out of 5)
  - `votes` — Number of votes received
  - `approx_cost(for two people)` — Approximate cost for two people (₹)
  - `listed_in(type)` — Restaurant category (Buffet, Cafes, Dining, Other)

##  Tools & Libraries Used
- **Python**
- **Pandas** — data manipulation
- **Matplotlib** — data visualization
- **Seaborn** — statistical visualization

##  Analysis & Key Insights

| # | Analysis | Visualization | Insight |
|---|----------|----------------|---------|
| 1 | Restaurant type distribution | Count plot | Majority of restaurants fall into the **Dining** category |
| 2 | Votes by restaurant type | Line plot | **Dining** restaurants received the highest number of votes |
| 3 | Ratings distribution | Histogram | Most restaurants are rated between **3.5 and 4.0** |
| 4 | Average cost for two | Count plot | Majority of couples spend around **₹300** per order |
| 5 | Online vs Offline ratings | Box plot | **Online orders** received noticeably higher ratings than offline orders |
| 6 | Restaurant type vs order mode | Heatmap | **Dining** restaurants primarily receive **offline** orders, while **Cafes** primarily receive **online** orders |


##  Conclusions
- Dining restaurants dominate in both count and total votes, making them the most popular restaurant category.
- Customer ratings are concentrated in the 3.5–4.0 range, indicating generally positive but not extreme sentiment.
- Couples tend to prefer budget-friendly restaurants (~₹300 for two).
- Online ordering is associated with better customer ratings — a potential area to encourage more online adoption for offline-heavy segments.
- Since Dining restaurants receive more offline orders, Zomato can target these restaurants with promotional online-ordering offers to boost online conversions.

##  How to Run
1. Clone/download this repository.
2. Install dependencies:
   ```bash
   pip install pandas matplotlib seaborn
   ```
3. Open the Jupyter Notebook (`.ipynb`) file and run all cells.

##  Project Structure
```
├── zomato_dataset.csv         # Raw dataset
├── Zomato_EDA_Analysis.ipynb  # Jupyter notebook with full analysis
├── images/                    # Dataset & visualization snapshots
│   ├── dataset_snapshot.png
│   ├── 1_restaurant_type_countplot.png
│   ├── 2_votes_by_type_lineplot.png
│   ├── 3_ratings_distribution_histogram.png
│   ├── 4_cost_for_two_countplot.png
│   ├── 5_online_vs_offline_boxplot.png
│   └── 6_type_vs_order_mode_heatmap.png
└── README.md                  # Project documentation
```
