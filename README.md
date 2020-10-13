# Rubik's Cube Solver

#### `Systems`, `Parallel Computing`
Mentor: [@harshagrwl](https://github.com/harshagrwl) (+91 9582885426)

### Problem Statement
Given an arbitrary scrambled Rubik’s Cube, you need to implement a program that determines and finds the sequence with the fewest number of moves required to solve it.

### Description
The Rubik’s cube is a difficult puzzle because the decision tree for it rapidly increases in breadth. Consider a standard 3*3 Rubik's Cube. Basically we can perform 12 Quarter Turns (90 Degree turns) on any arbitary state of the cube.
It is known and has been proven that for this definition of a turn, the maximum number of moves required to solve a 3x3 cube is 26 moves. This is also known as [God's Number](https://cube20.org/qtm/). Therefore we can say that we have 26 states and 12 moves for each, this implies we need to compute 26¹² states in worst case to get our solution.

This is really time consuming and requires high computational power. We need to come up with a solution where we can try to divide our exploration task and let them run at the same time parallely. Here the Parallel Computing comes into picture.

You have to implement the Rubik's Cube solving algorithm using Parallel Processing. You are free to use any framework (OpenMP, MPI, CUDA).


### Useful resources:
- [Solving the Rubik's Cube using Parallel Processing - Paper](https://rc.library.uta.edu/uta-ir/bitstream/handle/10106/253/umi-uta-1179.pdf?sequence=1&isAllowed=y)
- [Algorithms for solving Rubik's Cube - Paper](https://arxiv.org/pdf/1106.5736.pdf)
- [OpenMP Tutorial](https://computing.llnl.gov/tutorials/openMP/)
- [MPI Tutorial](https://computing.llnl.gov/tutorials/mpi/)
- [CUDA Tutorail](https://cuda-tutorial.readthedocs.io/en/latest/)
- Refer to related resources for parallel computing framework of your choice.

### Bonus Task
If we carefully observe, we don't actually need to visit all the different states and explore them completely. Try to come up with an approach where we can try to reduce our search space by eliminating some of the states and thereby not exploring them. This can enhance and optimise our solution.

### Tips
- Document *at least* the following in your README - Description, Framwork Used, Setup Instructions, Screenshots (if any).
- The emphasis of the task is to understand and implement Parallel Computing concepts: Prioritize on learning the Parallel Computing part even if you are not able to come up with any optimized Algorithm.
- The Bonus task is *optional* and should be undertaken if you have completed the main task. However it is highly recommended to attempt both. 
