# Kohonen-Self-Organizing-Maps

## Function for updating weights of the Self-Organizing Map

*   The function takes SOM grid, training instance shade, learning rate (α) of the kth epoch, spread radius of the neighborhood of the winning node (σ) of the kth epoch, coordinates of the winning unit (x,y) in the SOM grid.
*   Neighbor units are selected using the neighborhood radius (σ) and only these units' weights are updated.
*   The weights of neighbor units of winning unit are influenced inversely proportional to their distance from the winning node. This neighbor units weight updation is carried using the **gaussian rule**. Closer the neighbor unit to the winning node more the change in its weight.

## Training function for the Self-Organizing Map (SOM)


*   Every epoch, the SOM is trained for all 24 shades.
*   Every epoch, the decay rate of the adaptive learning rate and the adaptive neighborhood radius is proportional to current number of iteration. Thus, the learning rate and the radius decreases as the epochs increase. 
*   Every epoch, the training data of 24 colors are shuffled just to introduce some randomness in which shade is mapped first. This just done for the sake of fairness. 
*   Every epoch, for each training example (from the 24 shades) the best/winner node is selected via the function "select_winning_node" and then after finding the winner unit, the weights of the map are updated using the function "update_weights" 

## Training function for the Self-Organizing Map (SOM)


*   Every epoch, the SOM is trained for all 24 shades.
*   Every epoch, the decay rate of the adaptive learning rate and the adaptive neighborhood radius is proportional to current number of iteration. Thus, the learning rate and the radius decreases as the epochs increase. 
*   Every epoch, the training data of 24 colors are shuffled just to introduce some randomness in which shade is mapped first. This just done for the sake of fairness. 
*   Every epoch, for each training example (from the 24 shades) the best/winner node is selected via the function "select_winning_node" and then after finding the winner unit, the weights of the map are updated using the function "update_weights" 

## Conclusion 

*   As the SOM is trained with increasing number of epochs, the center for each color are intensified.
*   Increasing the sigma value (neighborhood radius), the resultant SOM grid wil have clear different colors with smooth transitions.
*   As the numner of epoch increases the output is sharper. The boundary of each color is more visible. 
*   As we can see in the output of the sigma value = 10 as the number of epoch increases the colors are spread out widely. 
*   With the increase in the sigma value the region affected by the training example increases as we can see in the first row with sigma value = 1 there are no regions created regardless of the increase in the number of training epochs.
*   Sigma value increase the transition of colors is smoother compared to the output of the lower sigma value.







