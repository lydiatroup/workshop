## Response to Stevens
3/2/2020

1) The estiamation technique used in this article utilizes the random forests model. This model encorporates remote sensing and geospatial
data from multiple scales and combines it with census data to estimate the population density for each grid in a given area. The
random forest model utilizes machine learning to create increasingly accurate models. In the article Random Forest was used in R. First,
covariates are identified and then used to create a forest of trees within a country, each tree representing the log population density
for a given pixel. It was found the most accurate model was found by taking the mean of all trees in a forest and undoing the log to
find an estimated population density.

2) The random forest model discussed is a machine learning algorithm. This means the model "improves upon bagging," meaning it becomes
more and more accurate each time it is run. Overall, the random forest model is similarly accurate to classical regression statistical
models, but has the advantage of returning fewer values making it easier to interpret. The article states the random forest model
performs better than other map modeling methods for population density.

3) Covariates are information about the population, such as the country being measured, which may impact the final outcome. They're similar to confounding variables in science. Distance based covariates are mentioned throughout the article, which includes things like police stations. There likely would be a higher popultion around a police station than in areas without one, the same goes for hospitals or government buildings. Covariate data is blended with census data and other big data sets to create a more accurate model. This occurs through the combination of hard count data, census data, and more uncertain data, covariates.

4) It is imporant to have a highly accurate description of where all people live in the world, especially in LMICs. Traditional census and population counting techniques are very hard to make accurate in LMICs, partly because it is harder to reach people, and partly because it is harder to estimate where people are. Population estimation methods, such as random forests, can help to solve this problem by accurately modeling population density. Additionally, it is important to have a data set modeling population for the enitre population at one data scale. If the population model utilized different data scales in different countries, it would be harder to compare them to eachother, however when it is all produced on a country or continental scale, it is easier to make accurate comparisons.

5) In order to smartly allocate aid for human development, one must know where people in LMIC are concentrated, so they can target the corrrect groups. Inaccurate population models often exclude those that need aid the most. In Belize this type of population model will help uncover the counts of those living in less developed regions, indicating where to distribute aid and human migrant patterns. It would be especially insightful to track how population density changes in the districts consitinging primarily of rainforests.
