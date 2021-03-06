# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: I have completed the extra function, naked_twins, and added it to the main solve loop.
This function finds all the boxes with two digits, then for each of those boxes, checks each unit that the box belongs to,
to see if there is another box with the same value. If there is then it loops through all the other boxes in that unit and
removes the digits.
All the unit tests pass, but I'm pretty sure this isn't the most effective way to do this. I'm new to python, and still don't fully know the language features. It would be great to see a text book answer.



# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: I have added an extra set of 'units' that include the two main diagonals. These two units are included in the
unit list and then used as peers in the other functions. This means that the ```eliminate()``` and ```only_choice()``` functions,
will automatically include them.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project.
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve.
