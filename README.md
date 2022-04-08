# PyZADR
Python module for the Zero Adjusted Dirichlet Regression model based on PyMC

## Dataset branch
The `dataset` is a branch to share datasets publicly. The details are described in a supplemental document for the manuscript: *The United States-China Trade War and Impact on the Post Conservation Reserve Program Land Allocation*

1. Relevant Information:
   
   The eight datasets were created in the above manuscript, using the various prices, acres planted, yields, and costs samples of agricultural activities. In the original data ([raw_dat](raw_dat.csv)), there are seven covariates and corresponding dependent variables, along with the two spatial and temporal attributes. The covariates are the expected land net returns from the seven agricultural activity categories: corn, soybeans, wheat, other crops, pasture/range, forest, and other activities. The dependent attributes are land-use shares transitioning from the Conservation Reserve Program (CRP) to different activities.
   
   The rest of the datasets were derived from the original data. Each data consists of one land-use share returning to one of the activities from the CRP and a corresponding own net return and absolute differences between own and other net returns.

2. Number of Instances (Observations): 35

3. Number of Attributes (Variables)
   - The original dataset: 7 covariates and 7 dependent variables with spatial and temporal attributes
   - Rest of others: 6 covariates and 1 dependent variable with spatial and temporal attributes
   
4. Attribute Information:
     
  | Attribute type     | Attribute name     | Description                                                |
  |--------------------|--------------------|------------------------------------------------------------|
  | Dependent variable | NRTN_CORN          | Five year average of net return for corn production        |
  |                    | NRTN_SOYBEANS      | Five year average of net return for soybean production     |
  |                    | NRTN_WHEAT         | Five year average of net return for wheat production       |
  |                    | NRTN_OTHER_CROPS   | Five year average of net return for other crop productions |
  |                    | NRTN_PASTURE/RANGE | Five year average of net return for pasture and range      |
  |                    | NRTN_FOREST        | Five year average of net return for forest                 |
  |                    | NRTN_ALLOTHERS     | Five year average of net return for other activities       |
  | Covariate          | LUSHR_CORN         | Land-use share returning to corn production                |
  |                    | LUSHR_SOYBEANS     | Land-use share returning to soybean production             |
  | Spatial            | FP_REGION          | Farm production regions in contiguous US                   |
  | Temporal           | QUINQUENNIUM       | 5-years period between 1992 and 2017                       |


5. Sources
   
   Calculated by Meongsu Lee (University of Missouri) in 2021 from the following original sources:
   - Dubois M.R., C.B. Erwin, and T.J. Straka. "Costs and Cost Trends for Forestry Practices in the South." Forest Landowner 60, 2(2001): 3--8.
   - Dubois M.R., T.J. Straka, S.D. Crim, and L.J. Robinson. "Costs and Cost Trends for Forestry Practices in the South." Forest Landowner, (March/April 2003).
   - Moulton, R.J. and K.R. Richards. "Cost of Sequestering Carbon through Tree Planting and Forest Management in the United States." GTR WO-58. Washington, DC: U.S. Department of Agriculture, Forest Service (USDA-FS), 1990.
   - Smidt, M.F., M.R. Dubois, and B.S. Folegatti. "Costs and Cost Trends for Forestry Practices in the South." Forest Landowner, (March/April 2005).
   - Folegatti, B.S., M.F. Smidt, and M.R. Dubois. "Costs and Cost Trends for Forestry Practices in the South." Forest Landowner, (September/October 2007).
   - Barlow, R.J., M.F. Smidt, J.Z. Morse, and M.R. Dubois. "Cost and Cost Trends for Forestry Practices in the South." Forest Landowner, (September/October 2009).
   - Barlow, R.J., and M.R. Dubois. "Cost and Cost Trends for Forestry Practices in the South." Forest Landowner, (November/December 2011).
   - Dooley E., and R.J. Barlow. "Special Report: 2012 Cost and Cost Trends for Forestry Practices in the South." Forest Landowner, (July/August 2013): 22--28.
   - Maggard A., and R.J. Barlow. "Special Report: 2016 Costs and Cost Trends for Southern Forestry Practices." Forest Landowner, (September/October 2017): 31--39.
   - Smith, J.E., L.S. Heath, K.E. Skog, and R.A. Birdsey. "Methods for Calculating Forest Ecosystem and Harvested Carbon with Standard Estimates for Forest Types of the United States." GTR NE-343. Washington, DC: USDA-FS, 2005.
   - U.S. Department of Agriculture, Forest Service (USDA-FS). "Forest Products Cut and Sold from the National Forests and Grasslands." Washington, DC: USDA-FS, 2020. [https://www.fs.fed.us/forestmanagement/products/cut-sold/index.shtml](https://www.fs.fed.us/forestmanagement/products/cut-sold/index.shtml).
   - _______. "The Forest Inventory and Analysis Database." Washington, DC: USDA-FS, 2020. [https://www.fs.fed.us/emc/rig/DATIM/index.shtml](https://www.fs.fed.us/emc/rig/DATIM/index.shtml).
   - U.S. Department of Agriculture, National Agricultural Statistics Service (USDA-NASS). "Quick Stats Agricultural Database." Washington, DC: USDA-NASS, 2021. URL: [https://quickstats.nass.usda.gov](https://quickstats.nass.usda.gov).
   - U.S. Department of Agriculture, Natural Resource Conservation Service (USDA-NRCS). "Web Soil Survey." Washington, DC: USDA-NRCS, 2018. URL: [https://websoilsurvey.nrcs.usda.gov/](https://websoilsurvey.nrcs.usda.gov/).
   - _______. "2012 NRI - Movement of CRP land out of CRP by land cover/use." Washington, DC: USDA-NRCS and Ames, Iowa: Center for Survey Statistics and Methodology, 2017.
   - _______. "2017 NRI - Movement of CRP land out of CRP by land cover/use." Washington, DC: USDA-NRCS and Ames, Iowa: Center for Survey Statistics and Methodology, 2021.
   - _______. "Summary Report: 2017 National Resource Inventory." Washington, DC: USDA-NRCS and Ames, Iowa: Center for Survey Statistics and Methodology, 2020. URL: [https://www.nrcs.usda.gov/wps/portal/nrcs/main/national/technical/nra/nri/results/](https://www.nrcs.usda.gov/wps/portal/nrcs/main/national/technical/nra/nri/results/).
