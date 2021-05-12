### Business Requirements

  1. Clean up the Model field to leave only the letters to represent the Brand of the bike
To remove only letters under the Brand of the bike column, use clean > remove numbers only
  2. Workout the Order Value using Value per Bike and Quantity
Create Calculated Field > Value per Bike * Quantity = Order Value (new column) 
  3. Aggregate Value per Bike, Order Value and Quantity by Brand and Bike Type to form:
     1. Quantity Sold
     2. Order Value
     3. Average Value Sold per Brand, Type
On the flow area, create a new Aggregate step > drag columns Brand and Bike Type under Group Fields. Place Order Value, Quantity Sold and Value per Bike under Aggregate Field 
  5. Calculate Days to ship by measuring the difference between when an order was placed and when it was shipped as 'Days to Ship'
Create Calculated Field > Shipping Dates - Order Dates = Days to Ship (new column) 
  6. Aggregate Order Value, Quantity and Days to Ship by Brand and Store to form:
     1. Total Quantity Sold
     2. Total Order Value
     3. Average Days to Ship
 
https://preppindata.blogspot.com/2021/01/2021-week-2.html
https://www.youtube.com/watch?v=0VBD5mNAvLg
https://community.tableau.com/s/group/0F94T000000gQqoSAE/preppindata
