# Minesweeper Solver with knowledge bases

In this project, the utility function is implemented to find the optimal policy to find the safest square to uncover by computing each of the adjecent squares' probabilities.

### Improved Agent (better performance than basic agent)

1. To find the safest square in terms of discovering the adjecent squares that are inferenced from the discovered square, each of the squares has to be computed by using the probability inference and the risk inference.

2. The probabilitiy inference computes all the possible probabilities by inferencing discovered squares. Each of the discovered squares has up to eight adjecent squares with the number of mines that are surrounded. Hence, the probabilities of the adjacent squares are equal, but each square will sum up the other probabilities that can be computed by the other discovered squares. 

3. The risk inference is the function by using the concept of 'what if' hypothesis. If one of the sequentially selected adjacent squares decides the other squares' identifications by considering the square as mine or clear square, then this situation is considered as risk free stage.
    - i.e) if you have 100 percent certainty to decide unreaveled adjacent squares by identifying one of the adjacent squares as mine or safe, then it is the risk free situation and immediately uncover all the adjacent squares.

### Please check the Minesweeper Analysis for the further details.
