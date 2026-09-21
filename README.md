# Modelamiento Dinámico del Cometa 3I/ATLAS: Martian Perturbation Pipeline

[![Journal](https://shields.io)](https://elsevier.com)
[![ORCID](https://shields.io)](https://orcid.org)

This repository hosts the coupled, high-precision orbital mechanics pipeline and sensitivity integration matrices utilized to model the hyperbolic transit of the interstellar object **3I/ATLAS** under continuous outgassing forces and multi-body gravitational fields. 

This computation architecture supports the research manuscript submitted to the Elsevier journal ***Astronomy and Computing***.

## 🧮 Numerical Framework & Physics

Unlike standard uncoupled n-body routines, this software pipeline features a simultaneous state-vector integration system. It couples the Newtonian gravitational attraction of the primary star and the direct/indirect perturbations of Mars alongside time-dependent non-gravitational mass-loss curves ("rocket effect").

### Key Algorithmic Features:
* **Integrator Engine:** 5th-order Dormand-Prince Runge-Kutta adaptive step algorithm (SciPy `solve_ivp` RK45 method).
* **Local Precision Constraints:** Relative and absolute error tolerances fixed tightly at 10⁻¹⁰ to prevent specific energy truncation drifts over a simulated temporal envelope of 160 days.
* **Sensitivity Matrix Evaluated:** Core bulk density configurations explored across realistic cometary aggregate boundaries (\(\rho \in \{400, 500, 600\} \text{ kg/m}^3\)) to map cross-sectional non-linear trajectory drifts.

## 📂 Code Architecture

* `martian_perturbation_pipeline.py`: Main executable production-ready Python script holding the ODE systems, initial state vector conditions, and sensitivity looping matrices.
* `requirements.txt`: Environment definitions listing exact scientific computing library dependencies.

## 🚀 Dependencies and Execution

To deploy the coupled integrator array, initialize an environment with the following dependencies:

```bash
pip install numpy scipy matplotlib
```

## 🎓 Author & Open Science Compliance

* **Author:** René Sagal Andrade
* **Affiliation:** Independent Researcher / Aerospace Architect & Astro-aerospace Analyst
* **Academic Background:** University College London (UCL) Alumnus
* **Identifier:** [ORCID: 0009-0006-8968-301X](https://orcid.org)

*The author explicitly acknowledges the computational validation framework and algorithmic workflow support provided by Google's Smart Mode workflows during the development of this independent numerical pipeline.*
