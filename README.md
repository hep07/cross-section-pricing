# cross-section-pricing
Try to use ML to solve the cross sectional problem in Asset pricing 

R code is used to download CRSP monthly data and Compustat Yearly and Quarterly data from WRDS and merge them into CCM files. Ideally we would only use quarterly and the most recent 40 years of data maybe. 

These cleaned data served as input to this python project

The python code in this project analyze the data and try to use NN and gradient boosting to try to 
1) predict which stock will have larger alpha w.r.t. traditional FF 3 factors plus momentum and construct a long short portfolio based on the alpha prediction. To be precise, the Y variable is the residual from FF3 
2) Predict the raw return and based on the raw return form a long short portoflio 

1) may have the advantage of closer to ideal i.i.d. case while in fact we have a panel data. 

