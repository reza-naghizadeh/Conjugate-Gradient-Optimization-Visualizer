# Conjugate Gradient Optimization Visualizer

This repository contains a MATLAB implementation of the **Conjugate Gradient Method** for optimizing a quadratic function. The script visualizes the optimization process using a contour plot, showing the convergence path to the function's minimum point.

This code was developed as part of our Optimization course project at IASBS, in collaboration with my groupmate, [Erfan Faridi](https://github.com/erfanfaridii/).

## Features

- **Contour Plot Visualization**: Displays the contour plot of the quadratic function and tracks the optimization path.
- **Gradient and Hessian Computation**: Calculates gradients and Hessians symbolically for accuracy.
- **Adaptive Learning Rate**: Dynamically updates the learning rate at each iteration.
- **Convergence Criteria**: Stops iterating when the solution converges within a specified tolerance.
- **Detailed Output**: Displays the number of iterations, the minimum point, and the function value at the minimum.

## Prerequisites

- MATLAB R2016b or later.
- Symbolic Math Toolbox.

## Getting Started

### Clone the Repository
```bash
git clone https://github.com/username/Conjugate-Gradient-Optimization-Visualizer.git
cd Conjugate-Gradient-Optimization-Visualizer
```

### Run the Script

1. Open `conjugate_gradient_visualizer.m` in MATLAB.
2. Run the script.

### Output

- The script will display:
  - The number of iterations taken to converge.
  - The coordinates of the minimum point.
  - The minimum value of the function.
- A contour plot with the optimization path overlaid will be generated.

## Customization

- **Initial Point**: Modify the initial point `x` in the script:
  ```matlab
  x = [-2; 2.5];
  ```

- **Tolerance**: Adjust the stopping criteria by changing the tolerance in the iteration loop:
  ```matlab
  if (errorAmountx1 < 10e-8 && errorAmountx2 < 10e-8)
  ```

- **Function**: Replace the function `f` with your own:
  ```matlab
  f(x1, x2) = (10 * x1 ^ 2) - (4 * x1 * x2) + (x2 ^ 2);
  ```

## Example Output

The script minimizes the function:

\[ f(x_1, x_2) = 10x_1^2 - 4x_1x_2 + x_2^2 \]

and outputs the minimum point and value, while displaying a contour plot with the optimization path.


## Acknowledgments

- MATLAB Documentation: [Symbolic Math Toolbox](https://www.mathworks.com/products/symbolic.html)
- Conjugate Gradient Method: [Wikipedia](https://en.wikipedia.org/wiki/Conjugate_gradient_method)
