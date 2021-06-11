### Business Requirements 
1) What's the Total Prize Money earned by players for each tour?  
Use aggregate with TOUR under Grouped Fields and MONEY under Aggregated Fields - Answers: 58,410,411 for LPGA and 256,726,356 for PGA

2) How many players are in this dataset for each tour?
Use aggregate with TOUR under Grouped Fields and PLAYER NAME under Aggregated Fields - Answers: 100 players for LPGA and 100 players for PGA

3)How many events in total did players participate in for each tour?
Uuse aggregate with TOUR under Grouped Fields and EVENTS under Aggregated Fields - Answers: 2,266 for LPGA and 2,282 for PGA

4) How much do players win per event? What's the average of this for each tour? (help)
Create a new step then create a new calculated field to find out the money a player gets per event MONEY/EVENTS - Answers: Average Money Per Event for LPGA is $25,525 and $120,281 for PGA

5) How do players rank by prize money for each tour? 
Create a new clean step and use rank per TOUR using the MONEY column 

6) What about overall? 
Use rank using the MONEY column

7) What is the average difference between where they are ranked within their tour compared to the overall rankings where both tours are combined? 
Use aggregate with TOUR under Grouped Fields and Avg in Diff in Ranking under Aggregated Fields 

8)Here we would like the difference to be positive as you would presume combining the tours would cause a player's ranking to increase
Combine the answers to these questions into one dataset  
  a) Pivot the data so that we have a column for each tour, with each row representing an answer to the above questions
  b)Clean up the Measure field and create a new column showing the difference between the tours for each measure
  c)We're looking at the difference between the LPGA from the PGA, so in most instances this number will be negative
