### Business Requirements 
#### 1. Split the 'Store-Bike' field into 'Store' and 'Bike'
#### the first clean up step is a simple split value > automatic split. Two new columns appeared. Removed the original column. 
#### 2.Clean up the 'Bike' field to leave just three values in the 'Bike' field (Mountain, Gravel, Road) 
#### the second clean up step is a simple group value. 
#### 3. Create two different cuts of the date field: 'quarter' and 'day of month'  
#### The third clean up step is a simple Convert Dates to Quarter and Day of the Month 
#### 4. Remove the first 10 orders as they are test values  
#### The last clean up step is to remove the first 10 orders, to do so use the Order ID column > Filter > Range of Values > start from 11. 
#### 5. Output the data as a csv
