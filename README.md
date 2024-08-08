
# MLE for Weibull Distribution

This repository provides a detailed implementation of Maximum Likelihood Estimation (MLE) for the Weibull distribution. The Weibull distribution is a versatile distribution commonly used in reliability analysis and life data analysis. This repository includes both the theoretical derivation and practical implementation of MLE for estimating the distribution's parameters.

## Table of Contents

- [Overview](#overview)
- [Weibull Distribution](#weibull-distribution)
- [Maximum Likelihood Estimation (MLE)](#maximum-likelihood-estimation-mle)
- [Derivation](#derivation)
- [Implementation](#implementation)
- [Special Cases](#special-cases)
- [Examples](#examples)

## Overview

The Weibull distribution is widely used in various fields such as reliability engineering, weather forecasting, and survival analysis. This project focuses on deriving and implementing MLE for the Weibull distribution, enabling accurate parameter estimation from sample data.

## Weibull Distribution

The probability density function (PDF) of the Weibull distribution is defined as:

f(x; α, β) = (α / β) * (x / β)^(α - 1) * exp(-(x / β)^α)


where:
- `x > 0`: The variable of interest.
- `α > 0`: The shape parameter.
- `β > 0`: The scale parameter.

## Maximum Likelihood Estimation (MLE)

MLE is a method used to estimate the parameters of a statistical model by maximizing the likelihood function. For a sample `x1, x2, ..., xn` from a Weibull distribution, the likelihood function `L(α, β)` is given by:

```
L(α, β) = ∏ (f(xi; α, β))
```

The log-likelihood function, which simplifies the process, is:

```
ln L(α, β) = n ln α - n α ln β + (α - 1) ∑ ln xi - ∑ (xi / β)^α
```

## Derivation

This section provides a step-by-step derivation of the log-likelihood function for the Weibull distribution and details on how to compute the partial derivatives to estimate the parameters `α` and `β`. 

## Implementation

The repository includes Python code for:
- Deriving the MLE equations.
- Implementing the estimation process.
- Generating and visualizing the likelihood function for sample data.

## Special Cases

This section covers special cases where one of the parameters is known, simplifying the MLE process. It discusses the use of profile likelihood to estimate the remaining parameter.

## Examples

Examples of how to use the provided code to estimate the parameters of the Weibull distribution from sample data are included in the repository. This section also demonstrates comparison between full likelihood and profile likelihood estimations.


