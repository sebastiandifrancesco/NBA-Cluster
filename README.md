# NBA_Cluster

The purpose of this project was to create clusters of NBA players using their stats from the 2018-2019 season. The data was initially pulled from https://www.basketball-reference.com/. After cleaning the data and checking for outliers a heat map was generated to see which features correlated with other features:

![Image description](https://github.com/sebastiandifrancesco/NBA_Cluster/blob/main/heatmap.PNG)

After this a KMeans model was built using the statistics data. The model generated five different clusters:

![Image description](https://github.com/sebastiandifrancesco/NBA_Cluster/blob/main/cluster.PNG)

Cluster 2 seems to be the best players overall. It has players like James Harden, Giannis Antetokounmpo, and Lebron James. Cluster 0 seems to be players that are more offensively minded. They score their points off of a mix of 2-Point Field Goals and 3-Point Field Goals. This cluster includes players like Dennis Schröder, Kemba Walker, and Paul George. Cluster 4 appears to be players that are more defensively minded (lots of defensive rebounds, offensive rebounds, and highest number of blocks compared to all the other clusters). They also tend to score their points off 3_point Field Goals and have very low 2-Point Field Goals made. This cluster includes players like Kristaps Porziņģis, Tristen Tompson, and Dwight Howard. Cluster 1 appears to be the "bench warmers" and cluster 3 is like cluster 0 but on average is about twice as bad as scoring points as cluster 0.

Continuation of this work could include feeding the stats and the feature engineered clusters into a regression models to predict the players' salaries for the next year. To do this one would need to combine this data here with salary data pulled from somewhere off the web.
