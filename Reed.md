# Response to Reed: Gridded Population Maps Informed by Different Built Settlement Products

shows effectiveness of 3 high res built area datasets for gridden populatio estimates 
- binary dasymetric redistribution, random forest with dasymetric compondent, hybrid


2 main approaches to gridded population estimates
  1) top down: estimates start with census data then disaggregate pop into smaller units
      areal weighing (dist uniformly) -> GPW
  2) bottom up: calculating pop size from ancillary data
  daysemetric refines estimates by distributing pop into weighted ancillary feature class
  constrains where it gets reallocated to 
MODEL types
1) simplle binary daysemetric
    - census counts disaggregated into pixels coincident with built areas defined by given built product
    - clear boundary of built areas and ADMs
    
2) Random forest and daysymetric
    - population density-weighing surface based on RF model
    - 3 primary parameters: number of covariates, number of trees, number of observations
    - no visible boundary of built area or btwn ADMs
 
3) Hybrid
    - pop density weighing surface from model 2, restricts redist. of census data to built areas
i think its saying random forst models are better
