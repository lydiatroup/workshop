## Response to Nieves

Nieves et al. use the random forests model to predict population glovally. The Random Forest works by creating a number of decision trees to predict a certain variable. The decision tree is then applied to the data and the accuracy of it is measured. Then the weaker, less accurate trees are combined and improved, to create stronger, more accurate trees. In this paper, the RF model was used to model population density in low and low-middle income countries, and then applied to the census population units which were then redistributed using dasymetric modeling to estimate population counts.

  Dasymetric modeling provides important insights about the relationship between population and covariates. Daysymetric population allocation works to redistribute census population amounts into regions based on the predicted population densities found using the Random Forests model.
  
  This study found that globaly, covariates related to urban areas and topographic features were consistently the most important when comparing where people live. Additionally, there were some variations across regions. For example in central america non-residential land use covariates were found to be more important than the rivers/water/waterbodies covariates.


notes from Reading:
population increases in less developed countries  -> high rates internal/international migration. changes in spatial dist of pop = need more accurate high resolution spatial population maps for public health, policy, sustainability
human pop density correlated w/ environmental and physical factors

GPW- gridding of census data matched to ADMs
GRUMP - uses nightime lights
also LandScan, GHS-POP, WorldPop = multivariable approach
  only w/in country, none across low and middle income countries
Article: analysis for 32 low-income countries to answer: 1) what datasets most informative for mapping population dist, 2) differences in importance of datasets btwn countries, regions of/w/in coutries

Random Forest objects for each sample country trained at ADM level of census pop data, extrated covariate importance metrics, standardized what covariates rep, analyzed data for differences w/in covariate class and between spatial locations
Random forest is a ensemble method = takes 'weak learner' decision trees -> 'strong learners'
  here: select covariates, fit RF model -> make pop density weighing layer from it, redist of pop counts from census to grid cells using pop density from weighing layer
classified types of covariates into the table to facilitate comparision. landcover is generally good!
used weighted importance rank to rank covariates by importance / total # covariates in country (0 (most important) - 1(least))

lu - land use
RESULTS
covaraiates relating to urban areas and topographic features were most consisttently important!
  GLOBAL: built environment covariates, urban/suburban extents, climatic/environmental variables>>
  INTER-REGIONAL: only dif btwn regions : non residential LU variable, river/water/waterbodies variable. NON-residential LU more important in Central america
  INTRA-REGIONAL: C america / carribean: covariates w/ built environment, urban/suburban procies, transportation networks, urban/suburban extents, climatic/environmental variables better than river/waters
