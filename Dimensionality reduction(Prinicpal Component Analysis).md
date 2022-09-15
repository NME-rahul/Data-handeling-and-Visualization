- This pdf is a part of visualising associations among two or more quantity variables
 
## Dimension reduction with principal component analysis- 
Dimension reduction technique is used to perform the dataset consists of multiple correlated variables that convey overlapping information. Such dataset can be reduced to smaller dataset without loss of much critical information.
For example, consider a dataset of over 200 glass fragments. For each glass fragments, we have measurments about its composition, expressed as the the percentage in the weight of various mineral oxide. There are seven different oxides.

PCA - it introduces a new set of variables called principal components by linear combination of the original variables in the data, standardized to zero mean and unit variance. PCs are chosen such that they are uncorrelated and they are ordered such that the first component captures the largest possible amount of variation in the data and subsequent component capture increasingly less. 

![blue-jays-PCA-1](https://clauswilke.com/dataviz/visualizing_associations_files/figure-html/blue-jays-PCA-1.png  "dataset of blue jays birds")

When we perform PCA, we generally intrested in two pieces of information: (i) the composition of the PCs and (ii) the location of the individual data points in the pricipal components space.

First, we at look at the component composition. here, we only consider two componentes
PC1 - x axis
PC2 - y axis

![forensic-PCA-rotation-1](https://clauswilke.com/dataviz/visualizing_associations_files/figure-html/forensic-PCA-rotation-1.png "showing PCAs")

component one(PC1) measures primarily the amount of aluminium, barium, sodium, and magnesium contents in glass fragments(lines that are going along x axis).
component two(PC2) measures primarily the amount of calcium and potassium and to some extent amount of aluminium and magnesium(lines that are going along y axis).

Next, we project the original data into the prinicpal component space. we see a clear clustering of distinct tyes of glass fragments in this plot. by comparing this figure with above figure we can see that window samples tend to have higher than average magnessium contnet than average barium, aluminium, and sodium content, whereas the opposite is true for headlamp samples.

![forensic-PCA-1](https://clauswilke.com/dataviz/visualizing_associations_files/figure-html/forensic-PCA-1.png "original data clustered data")

