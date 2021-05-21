# Cryptocurrencies

## Overview
Cryptocurrency is a fairly new, complex, and vast field, with many different currencies and countless metrics that can be difficult to understand without proper analysis aided by visualizations. There is an opportunity to pitch an investment in cryptocurrencies to an accounting firm which could be quite lucrative. It will be necessary to analyze crypto data with the aim of discovering trends that can be used when pitching the investment.

## Resources

**Data Sources:**
[crypto_data.csv](https://github.com/GloriaY007/Cryptocurrencies/blob/main/Challenge/Resources/crypto_data.csv)

## Challenge Overview
In this example, an accounting firm is interested in offering a new cryptocurrencies investment portfolio for its customers. The task is to present a report of tradable currencies and how they can be grouped for classification in developing an investment product.

***Elbow Curve using hvPlot to find the best value for K***

![Elbow Curve using hvPlot](https://github.com/GloriaY007/Cryptocurrencies/blob/main/Challenge/Resources/elbow%20curve.png)

***Table with tradable cryptocurrencies***

![Tradable cryptocurrencies](https://github.com/GloriaY007/Cryptocurrencies/blob/main/Challenge/Resources/3D%20Scatter%20with%20PCS%20Data.png)

***hvplot scatter plot with x="TotalCoinsMined", y="TotalCoinSupply", and by="Class"***

![hvplot](https://github.com/GloriaY007/Cryptocurrencies/blob/main/Challenge/Resources/hvplot.png)

## Summary
First, the data needed to be transformed and scaled in order to be used by an unsupervised clustering algorithm. Due to the high degreee of features, PCA (Principal Component Analysis) was performed to identify the primary influences in variance of the data. Then, the K-Means Algorithm was deployed with 4 clusters (determined by an elbow curve) which classified the data entries into 4 groups. When we created the visuals, there seemed to be a clear outlier (Bittorrent) revealed, with the other three clusters having relatively clear boundaries between them. On the other hand, when we take a look at the original features 'TotalCoinsMined' vs. 'TotalCoinSupply', the clustering does not provide any particular insights into the cryptocurrencies' trends. Therefore, we would either need more features to be added or more data points to try and extract meaningful groupings.
