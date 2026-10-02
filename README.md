# Conditional Expectation and Bayes Prediction

Homework 2 for *Machine Learning: Mathematical Basis* (D.B. Rokhlin, SFEDU, 2026).

## Problem

Given X uniform on [-1, 1] and Z exponential with rate 1, independent of each other, and Y = X + Z, this assignment derives:

- The conditional density of Y given X
- The conditional mean and median of Y given X
- The Bayes predictors under squared loss and absolute loss
- The theoretical and empirical risk minimizers within the restricted family f_a(x) = x + a

## Key result

The family f_a(x) = x + a was deliberately chosen with slope 1 on x, matching the slope of both true Bayes predictors. As a result, minimizing the risk within this restricted family recovers the unconstrained Bayes predictor exactly rather than only approximating it.

- Squared loss: theoretical minimizer a = 1, matching the Bayes predictor x + 1
- Absolute loss: theoretical minimizer a = ln 2 (about 0.693), matching the Bayes predictor x + ln 2

A numerical experiment with n = 5000 simulated samples confirms both minimizers closely, within normal sampling noise.

## Files

- `HW2_theory.pdf`, full theoretical derivation (parts 1 through 4a)
- `HW2_NumericalExperiment.ipynb`, the numerical experiment verifying the theory (parts 4b and 4c), including plots and a comparison of empirical and theoretical minimizers

## Author

Goriola-Obafemi Babatunde Sukanmi, MSc Applied Mathematics and Informatics, SFedU
