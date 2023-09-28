# Birthday Paradox Probability Calculator

This Python notebook calculates the probability of at least two people sharing the same birthday in a room with a given number of people. It also includes a basic visualization of the accumulated probability.

![birthday_problem_cdf](https://github.com/Marlup/Birthday-problem/blob/main/birthday_problem_cdf.png)



## Table of Contents

- [Usage](#usage)
- [Code Explanation](#code-explanation)
- [Probability Calculation](#probability-calculation)
- [Probability Visualization](#probability-visualization)
- [Example Output](#example-output)
- [License](#license)


## Usage

1. Ensure you have Python and the required libraries installed (NumPy and Matplotlib).

2. Clone this repository to your local machine.

3. Run the Python Jupyter notebook to calculate and visualize the probabilities

The notebook will output the probabilities for different room sizes and display a plot showing the accumulated probability.

## Code Explanation

The code is divided into two parts:

### Probability Calculation

The first part of the code calculates the probability of at least two people sharing the same birthday for various room sizes. It follows these steps:

+ Set the period to 365, representing the number of days in a year.

+ Create a list cases containing the number of people in the room that you want to calculate the probabilities for.

+ Initialize an empty list Ps to store the calculated probabilities.

+ For each value n_agents in the cases list, the script calculates the probability of no one sharing a birthday and subtracts it from 1 to get the probability of at least two people sharing a birthday. The result is rounded to four decimal places.

+ The probabilities are printed to the console.

### Probability Visualization

The second part of the code visualizes the accumulated probability for different room sizes using Matplotlib. It includes:

+ A line plot of the accumulated probability.
+ Red dots on the plot indicating the probabilities when there are 23 and 41 people in the room.
+ Annotations showing the exact probabilities at those points.
+ Labels for the x and y axes.
+ A legend for the plot.

## Example Output

Here's an example of the output:

```python
  Probability of at least two matches in a room:

  If 1 people: 0.0
  If 3 people: 0.0082
  If 5 people: 0.0271
  If 7 people: 0.0546
...
```

## License

This project is licensed under the MIT License - see the LICENSE file for details.
