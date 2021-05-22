###Business Requirments

1. Union the Stores data together  
Use Wildcard to union all Stores data together, exclude the Target data

2. Remove any unnecessary data fields your Input step might create and rename the 'Table Names' as 'Store' 
Create a new clean step and renamed Table Names to Store

3. Pivot the product columns  
Create a new Pivot step and drag all the produc columns to the column. Make sure that it is set to columns to rows.

4. Split the 'Customer Type - Product' field to create:  
  Customer Type
  Product
  Also rename the Values column resulting from you pivot as 'Products Sold'
Use Split Value > Automatic 

5. Turn the date into a 'Quarter' number 
Use convert to quarter option

6. Sum up the products sold by Store and Quarter 
Create a new Aggregate step and drag Store and Quarter under Group Field , drag Product Sold under Aggregate Field 

7. Add the Targets data 
Drag Target data into the panel

8.Join the Targets data with the aggregated Stores data 
  Note: this should give you 20 rows of data
Join step 6 with step 7, join by Quarter and Store 

9. Remove any duplicate fields formed by the Join

10. Calculate the Variance between each Store's Quarterly actual sales and the target. Call this field 'Variance to Target' 
Create Calculated Field using the formula Product Sold - Target under a new column named Variance to Target

11. Rank the Store's based on the Variance to Target in each quarter 
Go to Variance to Target column > Create Calculated Field > Rank , Group by Quarter

12. The greater the variance the better the rank

https://www.prosvetova.com/page2/ 
