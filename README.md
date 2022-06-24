# Cryptocurrencies

## Overview of the analysis: 
The purpose of the analysis is to process data from CryptoCompare and fit it into the unsupervised machine learning models by using a clustering algorithm. Will be including data visualizations to share findings with the board interested in offering a new cryptocurrency investment portfolio for its customers.


## Results: 
The data file had 1252 rows

- 1144 rows were tradeable, however,

- 459 rows had NaN values under Total Coins Mine Column

- 153 rows did not have Coins Mined

This would leave 532 tradeable cryptocurrencies to work with.

After processing the data, reduced the data dimensions using PCA

the explained variance ratio is :

	
|    Pc 1    |    PC 2    |    PC 3    |
|            | -          | -          | 
| 0.02792992 | 0.02140785 | 0.02050050 |

To locate the number of clusters to initialize the K-Means model, the elbow method was used


![screen_1](/resources/Elbow_method.png)

3D - scatter plot with the PCA Data and the clusters

![screen_2](/resources/3dplot.png)

Processed the data again to scale the data to create a scatter plot with tradeable cryptocurrencies

![screen_3](/resources/bokeh_plot.png)


