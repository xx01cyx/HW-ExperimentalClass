To Do List
==========
- [x] Implement A* algorithm for Maze1 and Maze2
- [x] Fix `Clear` bug (disable the clear function when solving the maze)
- [x] Alert when the maze is unsolvable
- [x] Calculate and display the excecution time
- [x] Implement `Pause` when solving the maze
- [x] Fix the bug when Maze2 is ani-created (draw the maze from the top instead of from somewhere in between)
- [x] Set the canvas as empty when maze type changes
- [ ] Finish README.md

Notes
=====
* A priority queue is implemented to realize A* algorithm.
* H score could be calculated via different approaches: Manhattan distance, Euclidean distance, etc. The former is used in my code.
* Maze1 is definitely solvable while Maze2 is not. Therefore, an alert would pop up if no solution for Maze2 exists.
* Due to the synchronous execution of JavaScript code, `Promise` is significant to catch the error asynchronously thrown in another function, which **enables the alert** mentioned before.
* Calculation of the excecution time is realized via `performance.now()`.

