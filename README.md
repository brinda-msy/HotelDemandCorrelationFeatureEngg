# HotelDemandCorrelationFeatureEngg

In this section, the varaibles are analyzed for correlation and significance. 
Data cleaning 
      null value replacements ex - children 
      encoding string categorical variables ex - month, deposit type, customer type 
      Data type conversion from object into int 64 ex - deposit type, customer type 
      delete columns that have too many null values and distribution is too irregular ex - agent, company, country 
Correlation Analysis 
      Dependent variable - is_canceled 
      Predictor variables - this varies on the location. Each location has a different set of features that are more significant to the dependent variable 
      Pearson ceoff and p values are used to pick features for each location 
      Columns with low correlation and significance are dropped Ex - 'arrival_date_year','arrival_date_month'
      Columns with direct correlation are dropped to avoid model overfit Ex - 'reservation_status','reservation_status_date'
      
