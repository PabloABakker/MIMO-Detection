# MIMO-Detection

TU Delft project for the Master course **Applied Convex Optimization**.  
This project reframes the standard MIMO source separation problem as a relaxed convex optimization problem.

**Authors:**  
Inês Marques  
Pablo Bakker  

---

## MIMO Detection using Semidefinite Relaxation and PGD

This project implements QPSK MIMO detection using a Semidefinite Relaxation (SDR) of the Maximum Likelihood (ML) problem, followed by randomization techniques to recover discrete symbol decisions. A Projected Gradient Descent (PGD) method is also implemented as a faster alternative to solving the full SDP.

The system loads a simulated MIMO dataset, converts the complex model to a real-valued formulation, solves the relaxed optimization problem, and evaluates detection performance using Symbol Error Rate (SER) and Bit Error Rate (BER).

---

## Features

- QPSK MIMO system model  
- Complex-to-real system transformation  
- Semidefinite Relaxation (SDR) using CVXPY  
- Gaussian and Sphere randomization for discrete recovery  
- Projected Gradient Descent (PGD) solver  
- Performance evaluation: SER and BER  
- Convergence and timing analysis  

---

## Project Structure

├── MIMO_Detection.ipynb
├── Data/
│ └── mimo_detection.mat
└── README.md


---

## Requirements

Python 3.8+ is recommended.

Install dependencies:

```bash
pip install numpy scipy matplotlib cvxpy scs



