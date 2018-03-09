# Assignment 3, Part 2 - A Marbles Game

In a particular board game, there are N spaces in a row, numbered 0 through N - 1 from left to right. There are also N marbles, numbered 0 through N - 1, initially placed in their corresponding spaces. The single player begins by shuffling the marbles into a random order. After that, there are two moves available:

Switch: Switch the marbles in positions 0 and 1, and
Rotate: Move the marble in position 0 to position N - 1, and move all other marbles one space to the left (one index lower).
The objective is to arrange the marbles in order, with each marble i in position i.

### MarblesBoard

Write a class, MarblesBoard, to represent the game above. The class should be initialized with a particular sequence of Marbles in positions. Next, include switch() and rotate() methods to simulate the player's moves. Write a method, is_solved(), that returns True if the marbles are in the correct order.

Additionally, you may want to write __str__ and __repr__ methods that display the current state of the board. Your class should behave like the following example.
```
>>> board = MarblesBoard((3,6,7,4,1,0,8,2,5))  
>>> board
3 6 7 4 1 0 8 2 5  
>>> board.switch()  
>>> board  
6 3 7 4 1 0 8 2 5  
>>> board.rotate()  
>>> board  
3 7 4 1 0 8 2 5 6  
>>> board.switch()  
>>> board  
7 3 4 1 0 8 2 5 6
```
### Solver

Write a class, Solver, that actually plays the MarblesGame. Your class should take a MarblesBoard in its constructor. Write a solve() method that repeatedly calls the switch() and rotate() methods of the given MarblesBoard until the game is solved. However, you should not call switch when one of the two marbles being switched is 0. Given this limitation, your class should solve the game in the smallest possible number of moves.  
```
>>> board = MarblesBoard((1,3,0,2))  
>>> player = Solver(board)  
>>> player.solve()  
1 3 0 2
3 0 2 1
0 2 1 3
2 1 3 0
1 2 3 0
2 3 0 1
3 0 1 2
0 1 2 3
total steps: 7
```

### Validation
When you are done, check to see how many method calls (both switch() and rotate()) each of the following game boards require:

1. (5 2 1 0 3 4)

2. (3, 0, 8, 2, 6, 5, 4, 7, 9, 1)

3. (2, 10, 0, 9, 7, 11, 8, 5, 4, 6, 3, 1)

4. Compute the big O running time of your algorithm in terms of the number of Marbles:

	Select one:
	
	1. O(1)
	2. O(Log N)
	3. O(N)
	4. O(N Log N)
	5. O(N^2)
	6. O(N^3)
	7. O(2^N)
