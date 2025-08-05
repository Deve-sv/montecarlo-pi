# Monte Carlo Simulation: Estimating π

##  Overview
This project demonstrates how Monte Carlo methods can approximate the value of π by generating random points in a unit square and checking how many fall inside a quarter circle.

##  Method
- Generate N random points (x, y) uniformly in [0, 1] × [0, 1].
- Count points satisfying x² + y² ≤ 1 (inside the quarter circle).
- Estimate π as:
  
  π ≈ 4 × (Number of points inside / Total points)

As N increases, the variance of the estimate decreases, and the approximation converges toward the true value.

## Results
In this simulation, the number of points `N` is chosen randomly between 10,000 and 200,000 at each run.

Example simulation:

| Run | N (points) | Estimated π |
|-----|------------|-------------|
| 1   | 72,669     | 3.1488      |
| 2   | 156,912    | 3.1415      |
| 3   | 113,480    | 3.1382      |
| 4   | 85,247     | 3.1457      |

The random variation in `N` demonstrates that:
- The estimate remains close to the true value \( \pi \approx 3.1416 \).
- Increasing `N` reduces variance.
- Even with moderate values of `N`, the error is typically less than 0.5%.

## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/Deve-sv/montecarlo-pi.git
