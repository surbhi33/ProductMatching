# Data Extraction Process and ETA:

# Plan:
1. For our analysis, we would need to fuse two sets of data:
a. Shopee Data (Kaggle) - This includes images and text descriptions of different products (e.g. Shopping bags, luxury
clothes, exotic spices, etc.) available on the e-commerce website. Each product has multiple pictures and description
entries.
b. Ebay Data (scraping) - Similar data will be scraped from Ebay or other ecommerce websites in order to have
a more diverse set of data points (e.g. books, electronics, etc.).


# Pair Classification:
1. Make pairs of observations
2. Arrange some of the pairs to be from matching products (positive pairs)
3. Remaining pairs from non-matching products (negative pairs)
4. 1:1 Negative Sample is selected for maintaining class balance.
5. Train a binary classification model to take a pair and predict whether both observations belong to the same unique product or not. 
6. Cosine Similarity (used in Logistic) is calculated for all pairs and set as feature for model to find right distance. 
7. The models can be:
- Logistic regression
8. Neural Network
9. For any new observation, compare it with K nearest observations and classify.

![image](https://user-images.githubusercontent.com/46606885/160975277-f7b0975e-0747-4d4d-8610-2079190a6da0.png)
