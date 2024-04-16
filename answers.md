# CMPS 2200 Assignment 3
## Answers

**Name: Zoe Birnbaum**


Place all written answers from `assignment-03.md` here for easier grading.

1a) To solve this, we can start with the largest power of 2 that lies within N, subtract as many as possible of that number from N, move onto the next largest denomination, and so on, until the coins total to N. For example, if N=20, the least amount of coins we can use is 3 and these are their values: 8, 8, 4. 

1b) This algorithm is optimal because it selects as many of the largest 2^k coins as possible (greedy) before moving onto the next denomination. This reduces the amount of times a coin has to be picked, and each time a new coin needs to be picked presents a new problem of subtracting the next largest 2^k (optimal).

1c) Both the work and span are O(logn).



2a) If the coin denominations are 1, 3, 4 and N=6: The greedy algorithm would choose the largest denomination (4), and two of the 1 denominations, which results in 3 coins. However, the optimal solution only contains two coins of value 3. 

2b) This algorithm has an optimal substructure property which is the smallest possible number of coins to sum to N. 

2c) The work is O(N*k), as each subproblem multiplies the number of denominations by the "goal" number. The span is O(n).

