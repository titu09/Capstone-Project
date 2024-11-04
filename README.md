1. Project Name : Short Time Optimization For Amazon
2. Data Source : Kaggle
3. Dataset Link (CSV File) : https://www.kaggle.com/datasets/asaniczka/amazon-uk-products-dataset-2023
4. Data Information : 2.2M Amazon UK products data scrapped from October 2023
5. Features Within Dataset : asin, title, imgURL, productURL, stars, reviews, price, isBestSeller, boughtInLastMonth, categoryName
6. Features Overview : The features within dataset gives the information of 2.2M product's details as in the name of product, category it lies in, consumer satisfaction for the product, it's price and when it was bought
7. Project Goal : To use the hybrid models on the historic data for Amazon in order to obtain optimal prices. 
8. Benifits After Implementing The Model : The resulting optimal prices and other important features help in following -
(a) Revenue : optimal pricing help in increasing revenue thus improving net profitability 
(b) Price Elasticity : this parameter helps in understanding if increasing price of certain product won't affect sales of product yet improving profitability for that product
(c) Popularity Score : this parameter helps in monitoring consumer satisfaction throughout the time
(d) Market Growth : this parameter helps in understanding market growth throughout the time
(e) Inventory Turnover Rate : this parameter helps in understanding fast moving products or potential overstocking of products
9. Limitations Of Project : The datetime stamp is not present in the dataset, so the whole project depends on the arbitrary datetime created through feature engineering
10. Future Work : To get the dynamic real time data of Amazon (Amazon has blocked the access to fetch the data) and replace with statistical historic data, also resolve future unseen problems
11. How Is This Model Different From Amazon's Existing Model ?
    Ans : Amazon's existing model for optimizing prices uses various independent models in order to obtain robust model with good accuracy and achieve the goal while this project combines output of ARIMA model with robust ML models, and uses the predictions of best performing model in order to obtain optimal prices thus achieving same goal but reducing possible LOC while making more robust due to it's hybrid nature
13. Important Changes :
    (a) Data downsampled to 40% of data in order to resolve 'Pickling Error' for hypertuned Random Forest Regressor model
    (b) Replaced XGBoost regressor model with Light XGBoosting Machine regressor model so as to reduce runtime
14. Conclusion : Worked on historic amazon UK data obtained from Kaggle, implemented hybrid model to obtain predictions that further used with other important features help in obtaining optimal prices in order to improve profitability for the given historic dataset
