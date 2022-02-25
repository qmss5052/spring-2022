# KNN classification trials for cancer staging (by Toby)

Cancer staging information :
[https://www.cancer.gov/about-cancer/diagnosis-staging/staging](https://www.cancer.gov/about-cancer/diagnosis-staging/staging)

Procedure:
1. Retrieve mRNA expression profile, and TMN cancer staging data.
2. [Cleaning and merging](./sclc_ucologne_2015_data_cleaning.Rmd), removing samples without staging data, and genes without mRNA expression measurements. 
3. Cleaned data saved as [mRNA_levels_cancer_stage.txt](./mRNA_levels_cancer_stage.txt).
4. Basic KNN classifier training and testing in [Classification_for_TMN_stages.ipynb](./Classification_for_TMN_stages.ipynb)

Conclusions: 
- Simple KNN classifier seems able to determine whether cancer has metastasized (M staging), based on mRNA expression profile.
- However, performance is not so great for primary tumor and lymph node (T and N) staging.  
