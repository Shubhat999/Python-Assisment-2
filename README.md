# Python-Assisment-2
To solve this problem, we need to iterate through the players from left to right, keeping track of the tallest player we have seen so far. If we see a player taller than the tallest player we have seen so far, that player blocks Ali's line of sight, and we need to shoot the tallest player we have seen so far. After we have iterated through all the players, the tallest player we have seen so far will be the last player who blocks Ali's line of sight, and we need to shoot that player.

Algorithm:

Read the number of test cases T
For each test case do the following:
a. Read the number of players N and the height K of Gi-Hun and Ali.
b. Initialize a variable tallest to K (since Gi-Hun and Ali have the same height)
c. Initialize a variable shots to 0
d. Iterate over the heights of the players from left to right:
i. If the height of the current player is greater than tallest, increment shots and set tallest to the height of the current player
e. Print the value of shots
