# Ex.No: 3  Implementation of Minimax Search
### DATE: 09.03.24                                                                           
### REGISTER NUMBER : 212222060240
### AIM: 
Write a mini-max search algorithm to find the optimal value of MAX Player from the given graph.
### Algorithm:
1. Start the program
2. import the math package
3. Specify the score value of leaf nodes and find the depth of binary tree from leaf nodes.
4. Define the minimax function
5. If maximum depth is reached then get the score value of leaf node.
6. Max player find the maximum value by calling the minmax function recursively.
7. Min player find the minimum value by calling the minmax function recursively.
8. Call the minimax function  and print the optimum value of Max player.
9. Stop the program. 

### Program:


import math def minimax (curDepth, nodeIndex, maxTurn, scores,targetDepth): # base case : targetDepth reached if (curDepth == targetDepth): return scores[nodeIndex] if (maxTurn): return max(minimax(curDepth + 1, nodeIndex * 2,False, scores, targetDepth), minimax(curDepth + 1, nodeIndex * 2 + 1, False, scores, targetDepth))






### Output:

![WhatsApp Image 2024-04-27 at 10 36 53_99398dca](https://github.com/shridharshini8524/AI_Lab_2023-24/assets/148639799/f45f78bc-74d4-4a8c-83b3-c36ae67dabe6)




### Result:
Thus the optimum value of max player was found using minimax search.
