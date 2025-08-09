# Wings R Us – High-Performance Recommendation System

## Overview
Lookup-based item recommendation system with KMeans clustering fallback for non-repetitive and context-aware suggestions.  
8–10× faster than conventional machine learning recommenders while maintaining equal or better accuracy (Recall@3).

## Features
- Lightning-fast lookup algorithm
- KMeans-based fallback for unseen or rare combinations
- Context-aware: uses store, occasion, and customer type
- Word2Vec embeddings for semantic similarity
- CSV/Excel output
- Scalable and easy to maintain

## Installation
git clone https://github.com/saipy10/Gods_Codebase.git

cd Gods_Codebase

python -m venv venv

source venv/bin/activate    # Mac/Linux

venv\Scripts\activate       # Windows

pip install -r requirements.txt


## Data Requirements
Place the following CSV files inside the data/ folder:
- customer_data.csv — CUSTOMER_ID, CUSTOMER_TYPE
- store_data.csv — STORE_NUMBER, CITY, STATE, POSTAL_CODE
- order_data.csv — CUSTOMER_ID, STORE_NUMBER, ORDER_OCCASION_NAME, ORDERS JSON column

## How to Run
- Replace and enter correct dataset location
- Click on `Run All` in your notebook

## Output Format
CUSTOMER_ID,STORE_NUMBER,RECOMMENDATION_1,RECOMMENDATION_2,RECOMMENDATION_3
100001,17,"10 pc Grilled Wings Combo","8 pc Grilled Wings Combo","8 pc Spicy Wings Combo"
100002,12,"Classic Chicken Sandwich","Spicy Chicken Sandwich","Chicken Tenders"
