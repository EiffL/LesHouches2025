# Visualizations used in the lecture

## MCMC Banana Distribution (mcmc_banana.html)

Interactive visualization demonstrating Metropolis-Hastings MCMC sampling on a banana-shaped distribution.

**Features:**
- Visual representation of the target distribution (Rosenbrock function)
- Real-time animation of the sampling process
- Shows accept/reject decisions based on probability ratios
- Interactive controls for start/pause/reset and single-stepping
- Statistics panel with acceptance rates

**Usage in reveal.js:**
```html
<iframe src="visualizations/mcmc_banana.html" width="1200" height="800"></iframe>
```

## Maximum Likelihood Estimation - Gaussian Fit (gaussian_mle_optimization.html)

Interactive demonstration of Maximum Likelihood Estimation fitting a Gaussian distribution to non-Gaussian data.

**Features:**
- Real-time optimization using TensorFlow.js automatic differentiation
- Banana-shaped target distribution mimicking weak lensing degeneracies
- Live visualization of parameter evolution (mean vector and covariance matrix)
- Stable parameterization using tanh-constrained correlation coefficients
- Adaptive learning rate decay (10% reduction every 100 steps)
- 1σ and 2σ confidence contours with real-time updates
- Interactive controls for optimization (start/pause/reset/single-step)
- Statistics panel showing negative log-likelihood, parameters, and learning rate

**Technical Implementation:**
- Built with TensorFlow.js for automatic differentiation
- Numerically stable covariance parameterization to ensure positive definiteness
- Proper multivariate Gaussian log-likelihood computation with determinant terms
- Bounded standard deviations and constrained correlation parameters

**Educational Purpose:**
Illustrates the limitations of Gaussian approximations for complex posteriors, motivating the need for more flexible approaches like Simulation-Based Inference.

**Usage in reveal.js:**
```html
<iframe src="visualizations/gaussian_mle_optimization.html" width="1200" height="800"></iframe>
```
