
### Business Requirements

  1. Input the data source by pulling together all the tables
Use the wildcard to pull all the tabs from Excel to one table
  2. Pivot 'New' columns and 'Existing' columns

Create a new step with the Pivot option > Columns to Rows > drag all columns with 'New' and 'Existing' into the panel

  3. Split the former column headers to form:
     1. Customer Type
     2. Product
   
Use the Split Values > Automatic Split

  4. Rename the measure created by the Pivot as 'Products Sold'
  5. Create a Store column from the data
  6. Remove any unnecessary data fields
  7. Turn Date into Quarter

Use the Convert Date > Quarter

  8. Aggregate to form two separate outputs of the number of products sold by: 
     1. Product, Quarter - see Output2.csv
     2. Store, Customer Type, Product - see Output1.csv
Create two new clean steps, one is for Product, Quarter, the other is for Store, Customer Type, Product. Create two new Aggregate steps 
 
