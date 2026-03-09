<h1 align="center">Variance Reduction in Monte Carlo Simulations</h1>

<p align="center">
  <img src="https://img.shields.io/badge/R_Language-276DC3?style=flat-square&logo=R" alt="R">
  <img src="https://img.shields.io/badge/License-MIT-darkgreen?style=flat-square" alt="License">
</p>

<p align="center">
  <img src="../assets/banner.webp" alt="Banner" width="60%">
</p>

Monte Carlo simulations are powerful tools for estimating complex probabilistic quantities. However, they often suffer from high variance, which can limit their efficiency—especially when studying **rare events**. This project explores three major **variance reduction methods** designed to improve precision and reduce computational cost:

1. **Importance Sampling**: Modifies the sampling distribution to better capture rare events;
2. **Control Variates**: Leverages the correlation between random variables to reduce the estimator's variance;
3. **Stratification**: Segments the sampling space into homogeneous groups to refine estimates. 

The theoretical approach is complemented by a **real-world application in sports analytics**, evaluating the probability of an exceptional scoreline in a LOSC Lille (French football club) match.

---

## Resources

The report covers the following topics:
- Theoretical foundations of Monte Carlo simulations.
- Detailed presentation of variance reduction techniques.
- Mathematical proofs of fundamental properties.
- Performance benchmarking of these methods on concrete cases.
- Application to LOSC match data to estimate the probability of a victory by a margin of 8 goals or more.

| Document | Language | Link |
| :--- | :--- | :--- |
| Technical Report | English | [View PDF](../docs/Monte-Carlo-Variance-Reduction-EN.pdf) |
| Technical Report | French | [Read PDF](../docs/Reduction-Variance-Monte-Carlo-FR.pdf) |


## Code and Data
This project includes several **R** implementations (available in the [src/](../src/) directory):
- Estimation using Control Variates.
- Estimation using Stratification.
- Applied analysis of LOSC performance via Importance Sampling.

The variances associated with these methods are compared against the classic Monte Carlo approach.

**Data Used:**  
LOSC Lille match data (2005-2024), including goal difference calculations, can be accessed via the following link: [View CSV Data](../data/LOSC.csv)
  

## Installation and Usage

To explore the project locally:

```bash
# Clone the repository
git clone https://github.com/rmdair/Monte-Carlo-Variance-Reduction.git

# Navigate to the project directory
cd Monte-Carlo-Variance-Reduction
```

## References  
- Rasmussen & Glynn, *Stochastic Simulation: Algorithms and Analysis*, Springer, 2009.  
- Christian P. Robert & George Casella, *Monte Carlo Statistical Methods*, Springer, 2004.  
- Rubinstein & Kroese, *Simulation and the Monte Carlo Method*, Wiley, 2016.  
- Pour la Science (Scientific American French Edition), No. 385, Hasard et incertitude, les défis qu’ils posent, November 2009.