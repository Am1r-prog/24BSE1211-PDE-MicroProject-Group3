# 24BSE1211-PDE-MicroProject-Group3
# Quantum Confinement in a 1D Potential Well
**Course:** 24BSE2113-D – Partial Differential Equations, Transforms & Optimization Techniques  
**Department of Electronics and Communication Engineering**, Saintgits College of Engineering  
**Group:** 3

---

## Project Overview
This repository contains the complete analytical derivation and computational simulation of electron confinement in a 1D infinite potential box. Using the Time-Dependent Schrödinger Equation, we analytically derived the quantized energy eigenvalues, developed the Fourier series general solution, and built a Python simulation to plot the standing waves and probability distributions across states $n = 1, 2, 3$.

---

## Group Members & Contributions
* **Amir Mohammed N**: 
  * Core mathematical derivation of separation of variables and Dirichlet boundary condition proofs.
  * Formulation of the general time-dependent wave function using Fourier sine series.
  * Primary development of the Python simulation, NumPy vectorization, and Matplotlib visualizations in Google Colab.
  * Lead authoring of the LaTeX technical report and overall repository structure.
* **Amal Krishna S** (Group Leader): Initial repository creation, coordination, and submission management.
* **Robin Kirian Abraham**: Cross-verification of the energy eigenvalue formulas and intermediate derivation steps.
* **Harith C V**: Review of physical parameter values (effective mass, well dimensions) and testing code execution.
* **Hrishikesh S Nair**: Proofreading documentation, markdown styling, and reference compiling.

---

## Mathematical Summary

1. **Time-Dependent Schrödinger Equation ($V = 0$ inside well):**
   $$i\hbar\frac{\partial\Psi(x,t)}{\partial t} = -\frac{\hbar^2}{2m}\frac{\partial^2\Psi(x,t)}{\partial x^2}$$

2. **Quantized Energy Eigenvalues:**
   Applying the boundary constraints $\Psi(0,t) = \Psi(L,t) = 0$ yields:
   $$E_n = \frac{n^2 \pi^2 \hbar^2}{2mL^2}, \quad n \in \{1, 2, 3, \dots\}$$

3. **Stationary States & Probability Densities:**
   $$\psi_n(x) = \sqrt{\frac{2}{L}}\sin\left(\frac{n\pi x}{L}\right)$$
   $$|\Psi_n(x,t)|^2 = \frac{2}{L}\sin^2\left(\frac{n\pi x}{L}\right)$$

---

## Repository Contents
* `24BSE1211_PDE_MicroProject_Group_3.ipynb` — Google Colab notebook containing the Python simulation and inline plots.
* `README.md` — Project summary, individual contributions, and execution instructions.

---

## Running the Simulation
1. Open `24BSE1211_PDE_MicroProject_Group_3.ipynb` directly in Google Colab or Jupyter.
2. Ensure `numpy` and `matplotlib` are installed:
   ```bash
   pip install numpy matplotlib
