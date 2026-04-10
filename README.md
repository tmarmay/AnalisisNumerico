# Numerical Analysis

#### Tomas Marmay ~ FAMAF 2022

---

### Overview

Labs for the **Numerical Analysis** course at FAMAF. The course covers the fundamental algorithms of scientific computing: root finding, interpolation, numerical integration, and linear systems — all implemented from scratch in Python using NumPy and Matplotlib.

---

### Labs

| Folder | Topics |
|--------|--------|
| `lab1/` | Introduction: floating point arithmetic, error analysis |
| `lab2/` | Root finding: bisection, Newton-Raphson, fixed-point iteration |
| `lab3/` | Interpolation: Lagrange, Newton divided differences, climate data interpolation |
| `lab4/` | Least squares fitting, linear regression from scratch |
| `lab5/` | Numerical integration: composite trapezoid, midpoint, and Simpson's rules |
| `lab6/` | Linear systems: triangular solvers, Gaussian elimination, LU decomposition |
| `lab7/` | Linear programming with the simplex method (via `scipy.optimize.linprog`), Markov chains |

---

### Key Implementations

**Root finding (`lab2/`):**
- `newton.py` — Newton-Raphson method; takes a function `f(x)` returning `(f(x), f'(x))` and iterates until convergence.
- `rbisec.py` — bisection method with convergence tracking.
- `puntofijo.py` — fixed-point iteration.

**Interpolation (`lab3/`):**
- `newton_interpola.py` — Newton interpolation via divided differences table.
- `larange_interpola.py` — Lagrange interpolation.
- `clima_interpolacion.py` — applied interpolation on real climate data.
- Comparison plots between methods included.

**Numerical integration (`lab5/`):**
- `intenumcomp(fun, a, b, N, regla, error)` — unified interface dispatching to trapezoid, midpoint (`pm`), or composite Simpson.

**Linear systems (`lab6/`):**
- Lower-triangular solver (`soltrinf`), diagonal solver, and forward substitution — building blocks for LU decomposition.

---

### Exams

- `parcial/` — First midterm
- `parcial2/` — Second midterm (includes applied problem on Hurricane Irma trajectory data)
- `final/` — Final exam
