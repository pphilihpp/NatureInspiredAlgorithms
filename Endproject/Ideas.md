Clustering: 
Form clusters with exactly the capacity of the smallest vehicle.
Clusters can overlap. 


Idea:

  - Make a matrix of the customers "workmatrix" (indices are number of customer, value saved is the demand)
  - Starting with the customer that is most far away from the depot. 
  - Make a new array for the new cluster with number of customer and capacity. 
  - Look if the capacity of the car is more than full. 
    If not: 
  - Save the Customer number  and his demand in the new array. 
  - Set the value of the Customer number in "workmatrix" on 0. 
  - Go to next nearest neighbour of which the demand is not 0. Start over with looking if capacity is full.
    If so: 
  - Save customer + demand that makes the capacity full (capacity of car - capacity of vector before)
  - Set the demand value of the customer in "workmatrix" to the demand that is still needed. 
  - Create a new cluster and start again with customer that is most far away from depot and his demand is not 0. 
  
  
  
  
