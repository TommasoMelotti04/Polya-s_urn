# Polya's Urn Simulation

**Goal.** Simulate Polya’s Urn model and verify that the fraction of green balls converges in distribution to a uniform random variable on [0, 1].

---

## Problem Statement
An urn contains initially:
- `r = 1` red ball
- `g = 1` green ball  

At each time step:
1. Draw one ball at random.
2. Replace it.
3. Add `c = 1` additional ball of the same color.  

Let `X_n` be the fraction of green balls after the *n*-th draw.  

**Theoretical result:**  
As `n → ∞`, the random variable `X_n` converges in distribution to the **Uniform(0, 1)** distribution.

---

## Code & Simulation
The main implementation is available here:  
📓 [Polya.ipynb](Polya.ipynb)  

The notebook simulates the urn process and plots the empirical distribution of `X_n` compared with the uniform distribution.

---

## How to Run
```bash
pip install -r requirements.txt
jupyter lab
