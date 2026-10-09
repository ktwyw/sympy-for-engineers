# SymPy for Engineers

[![notebooks](https://github.com/ktwyw/sympy-for-engineers/actions/workflows/notebooks.yml/badge.svg)](https://github.com/ktwyw/sympy-for-engineers/actions/workflows/notebooks.yml)

Sixteen Jupyter notebooks that teach [SymPy](https://www.sympy.org/), Python's free computer
algebra system, through problems engineering students already meet in their courses: pipe flow,
beams, circuits, reactors, heat transfer, vibrations and control. Every exercise has a worked
solution, and the last notebook reproduces a published research result.

<img src="notebooks/double_pendulum.gif" alt="Double pendulum simulated from equations derived with SymPy" width="260" align="right">

Each example goes the whole way: **derive** the result symbolically, **verify** it against a
limiting case or an independent calculation, turn it into **numbers**, and **plot** it.

What SymPy is good for in engineering study:

- checking a hand derivation, or one produced by an AI assistant, before trusting it
- taking the algebra slips out of balances, boundary conditions and error propagation
- turning a derived formula into fast NumPy code, a fitted model, or C, Fortran and MATLAB code
- writing equations in LaTeX for a report without retyping them

The animation on the right is the last step of notebook 12, where the equations of motion are
derived from the energies in a few lines.

## The notebooks

Open any notebook in Google Colab with its badge. Nothing needs to be installed.

### Basics

| | Notebook | Engineering examples | |
| --- | --- | --- | --- |
| 1 | [Getting started](notebooks/01_getting_started.ipynb) | Reynolds number, Stokes settling velocity | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/01_getting_started.ipynb) |
| 2 | [Solving equations](notebooks/02_equations.ipynb) | distillation balance, van der Waals critical point, cubic equation of state, Colebrook friction factor | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/02_equations.ipynb) |
| 3 | [Calculus](notebooks/03_calculus.ipynb) | thermal expansion of a real gas, work of expansion, cantilever beam, critical radius of insulation, small-angle approximation | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/03_calculus.ipynb) |
| 4 | [Linear algebra](notebooks/04_linear_algebra.ipynb) | balancing reactions, mesh currents, natural frequencies, principal stresses, matrix exponential | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/04_linear_algebra.ipynb) |
| 5 | [Units and uncertainty](notebooks/05_units_and_uncertainty.ipynb) | unit conversion, dimensional checks, error propagation for a capillary viscometer, Monte Carlo check | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/05_units_and_uncertainty.ipynb) |

### Advanced

| | Notebook | Engineering examples | |
| --- | --- | --- | --- |
| 6 | [Differential equations](notebooks/06_differential_equations.ipynb) | Newton cooling, damped oscillator, Hagen–Poiseuille and power-law pipe flow, cooling fin, reactions in series | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/06_differential_equations.ipynb) |
| 7 | [Laplace transforms and Fourier series](notebooks/07_laplace_and_fourier.ipynb) | step responses, overshoot, dead time, closed-loop stability and ultimate gain, square wave | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/07_laplace_and_fourier.ipynb) |
| 8 | [From symbols to numbers](notebooks/08_symbols_to_numbers.ipynb) | `lambdify`, Langmuir fit with an exact Jacobian, large-amplitude pendulum, optimization, code generation | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/08_symbols_to_numbers.ipynb) |
| 9 | [Linearization and stability](notebooks/09_linearization_and_stability.ipynb) | draining tank, damped pendulum phase portrait, washout in a chemostat | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/09_linearization_and_stability.ipynb) |

### Showcase

| | Notebook | Engineering examples | |
| --- | --- | --- | --- |
| 10 | [Dimensional analysis](notebooks/10_dimensional_analysis.ipynb) | Buckingham pi groups by linear algebra: drag on a sphere, pipe flow, Nusselt–Reynolds–Prandtl, scaling an equation | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/10_dimensional_analysis.ipynb) |
| 11 | [Vector calculus](notebooks/11_vector_calculus.ipynb) | deriving the Laplacian in cylindrical and spherical coordinates, conduction in a spherical shell, potential flow around a cylinder, the centripetal term | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/11_vector_calculus.ipynb) |
| 12 | [Lagrangian mechanics](notebooks/12_lagrangian_mechanics.ipynb) | double pendulum: derivation, simulation, energy check, normal modes, chaos, animation | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/12_lagrangian_mechanics.ipynb) |
| 13 | [When SymPy fails](notebooks/13_when_sympy_fails.ipynb) | floats, assumptions, unsolvable integrals and equations, expression swell, loss of numerical accuracy, and the fix for each | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/13_when_sympy_fails.ipynb) |

### Going further

| | Notebook | Engineering examples | |
| --- | --- | --- | --- |
| 14 | [Partial differential equations](notebooks/14_partial_differential_equations.ipynb) | cooling of a slab, finite-difference formulas and their accuracy, method of lines, stability of time stepping, a nonlinear conduction code verified with a manufactured solution, steady conduction in a plate | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/14_partial_differential_equations.ipynb) |
| 15 | [Multibody mechanics](notebooks/15_multibody_mechanics.ipynb) | `sympy.physics.mechanics`: rotating frames, Lagrange's and Kane's methods, an inverted pendulum on a cart, its linearization and a controller that balances it, a rigid rod | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/15_multibody_mechanics.ipynb) |
| 16 | [Capstone: pipe flow of a Carreau–Yasuda fluid](notebooks/16_capstone_carreau_yasuda.ipynb) | the whole course on one research problem: an almost closed-form solution in hypergeometric functions, checked against limits, brute force and the published values of [Wang, JNNFM 310 (2022) 104937](https://doi.org/10.1016/j.jnnfm.2022.104937) | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ktwyw/sympy-for-engineers/blob/main/notebooks/16_capstone_carreau_yasuda.ipynb) |

Notebooks 1 to 5 should be read in order. After that, pick what matches your course. Notebook 13
is worth reading early: it explains most of the error messages a beginner will see. Notebook 16
assumes notebooks 2, 3, 6, 8, 10 and 13.

## Solutions

Every notebook ends with four or five exercises. The [`solutions/`](solutions) folder has a
notebook of the same name with a worked solution to each one, and every solution checks its
answer against an independent result.

Try the exercises before opening the solutions. If you teach with this material and would
prefer students not to have them, delete the `solutions/` folder from your copy; nothing else
depends on it.

## How each example is organized

1. **Problem**: stated as it would be in a textbook.
2. **By hand**: the outline of the derivation you are expected to know.
3. **With SymPy**: the same steps in code.
4. **Verify**: a limiting case, a known result, or an independent numerical check, written as an
   `assert` so that a wrong result stops the notebook.
5. **Numbers and a plot.**
6. **Exercises** at the end of each notebook, with worked solutions in `solutions/`.

SymPy is used here to check and extend hand derivations, not to replace them. If you cannot say
what the answer should look like, you cannot tell whether the computer's answer is right.

## Running the notebooks on your own computer

```bash
git clone https://github.com/ktwyw/sympy-for-engineers.git
cd sympy-for-engineers
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
jupyter lab
```

Python 3.11 or newer is required. The notebooks were built with Python 3.13, SymPy 1.14,
NumPy 2.5, SciPy 1.18 and Matplotlib 3.11.

## Testing

Every notebook and every solution is executed from top to bottom on each push, and once a
month, by [GitHub Actions](.github/workflows/notebooks.yml). To run the same check locally:

```bash
pip install -r requirements-dev.txt
pytest --nbmake notebooks/ solutions/
```

## Where to go next

- [SymPy documentation](https://docs.sympy.org/) and its
  [tutorial](https://docs.sympy.org/latest/tutorials/intro-tutorial/index.html)
- [carreau-yasuda-pipe-flow](https://github.com/ktwyw/carreau-yasuda-pipe-flow): the solution
  derived in notebook 16 as a Python library, command-line tools and a browser calculator
- [SymPy mechanics documentation](https://docs.sympy.org/latest/modules/physics/mechanics/index.html),
  for mechanisms beyond notebook 15

## Feedback

Corrections and suggestions for new examples are welcome through
[issues](https://github.com/ktwyw/sympy-for-engineers/issues).

## License

[MIT](LICENSE). Maintained by [Yanwei Wang](https://github.com/ktwyw), Nazarbayev University.
