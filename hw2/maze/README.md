Description
===========
A **webpage maze game** based on a [code base](https://github.com/zilinglius/maze), where some bugs have existed in the first place. 

Therefore, in my code, I try to 
1. Fix  the existing bugs
2. Add some new functions 
3. Improve the UI
   
**So [HERE](https://xx01cyx.github.io/Maze/) comes the maze game.** Click `How to play` button at the upper right corner of the page to get some instructions for the game. <br/><br/>
Enjoy your time!

To Do List
==========
- [x] Implement A* algorithm for Maze1 and Maze2
- [x] Fix clear bug (disable the clear function when solving the maze)
- [x] Alert when the maze is unsolvable
- [x] Calculate and display the excecution time
- [x] Implement pause as well as continue function when solving the maze
- [x] Fix the bug when Maze2 is ani-created (draw the maze from the top instead of from somewhere in the middle)
- [x] Set the canvas as empty when maze type changes
- [x] Enable selection of start point & end point in the 2nd canvas
- [x] Skip the animation of maze creating
- [x] Rewrite `maze.html`, using Bootstrap as CSS framework instead of Spectre
- [x] Add instructions for the game

Notes
=====
* A priority queue is implemented to realize A* algorithm.
* H score could be calculated via different approaches: Manhattan distance, Euclidean distance, etc. The former is used in my code.
* Maze1 is definitely solvable while Maze2 is not. Therefore, an alert would pop up if no solution for Maze2 exists.
* Due to the synchronous execution of JavaScript code, `Promise` is significant to catch the error asynchronously thrown in another function, which **enables the alert** mentioned before.
* Calculation of the excecution time is realized via `performance.now()`. However, The time calculated is not the actual run time of the algorithms, due to the execution characteristic of `requestAnimationFrame`.

Inspirations
============
* Use **deep learning** to estimate the cost of reaching goal from the current block. (Generated from BI054)
* Use **ray tracer** to simulate the transmission of light as search route. (Generated from my dream!)

Reference
=========
* [A* Pathfinding for Beginners](https://www.gamedev.net/reference/articles/article2003.asp)
* [JavaScript Toturial](https://www.w3schools.com/js/default.asp)
* [Bootstrap documentation](https://getbootstrap.com/docs/4.5/getting-started/introduction/)

