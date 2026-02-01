# Ising Model Simulations (Python)

Monte Carlo simulations of the Ising model using the Metropolis algorithm, with results visualised across different lattice sizes and external magnetic fields. The notebook explores 1D, 2D and 3D variants and compares to exact results where available.

## What this project covers
### 2D Ising model (B = 0)
- Metropolis Monte Carlo sweeps on an L×L lattice with periodic boundary conditions
- Magnetisation per spin plotted against temperature for multiple lattice sizes (L = 30, 40, 50, 60)
- Comparison to the exact 2D magnetisation curve (showing the critical temperature behaviour)

### 1D Ising model (with external field)
- 1D chain simulation for multiple system sizes (N = 8, 16, 32, 64)
- Magnetisation vs temperature for B = 0.1 and B = 0.5
- Comparison against the exact magnetisation expression provided in the assignment

### 2D energy and specific heat (with external field)
- Mean total energy vs temperature for multiple magnetic field strengths (B = 0.0, 0.2, 0.4, 0.6)
- Specific heat capacity vs temperature for multiple B values, including a reference line at Tc

### 3D Ising model
- Magnetic susceptibility vs temperature (3D lattice, B = 0)
- Magnetisation vs temperature for a range of magnetic field values

## Files
- `ising_model_simulation.ipynb` — main notebook containing code, plots and commentary
- `ising-questions.pdf` — assignment questions (relevant pages only)

## How to run
1. Install dependencies:
   - `numpy`
   - `matplotlib`
   - `numba` (used for speed via `@njit`)
2. Open the notebook and run all cells:
   - Jupyter Notebook / JupyterLab

## Notes on implementation
- Periodic boundary conditions are used in each model.
- Simulations include relaxation sweeps before measurements.
- Code is written to prioritise clarity and reproducibility, with labelled plots and readable functions.

## Tech
Python, NumPy, Matplotlib, Numba
