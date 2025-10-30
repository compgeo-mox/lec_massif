# Laboratory 2: Elasticity Equation

This lab focuses on the numerical solution of the elasticity equation using [PyGeoN](https://github.com/compgeo-mox/pygeon) and [PorePy](https://github.com/pmgbergen/porepy). The exercises cover the use of the Multi-Point Stress Approximation (MPSA) method using PorePy for elasticity. The main unknown is the displacement field $u$.

---

## Files Overview

- **ex1.ipynb**  
  *Rigid-body motion test for the elasticity equation on the unit square. The displacement is imposed as a rotation on the boundary. The solution and stress tensor are computed and exported for visualization.*

- **ex2.ipynb**  
  *Footing problem: vertical compression of a square domain with fixed bottom and a compressive force on the top. The stress tensor is post-processed and exported.*

- **ex3.ipynb**  
  *Cantilever beam problem: the beam is fixed on one side and subject to a body force. The displacement and stress tensor are computed and exported.*

- **ex4.ipynb**  
  *Cantilever beam problem with tensile force: the beam is fixed on one side and a tensile force is applied on the opposite side. The displacement and stress tensor are computed and exported.*

---

## Main Features

- **Elasticity equation**:

$$
\nabla \cdot [2\mu \epsilon(u) + \lambda \nabla \cdot u\, I] = -b
$$
  
  where $\epsilon(u)$ is the symmetric gradient, $\lambda$ and $\mu$ are Lamé parameters, and $b$ is a body force.

- **Boundary conditions**:  
  - Dirichlet (displacement) and Neumann (traction) conditions on various boundaries.
  - Rigid-body motion, footing, and cantilever beam scenarios.

- **Numerical methods**:  
  - MPSA (Multi-Point Stress Approximation) for general grids.

- **Post-processing**:  
  - Computation and export of stress tensor components.
  - Export of displacement fields for visualization in ParaView.

---

## How to Use

- Open each notebook (`ex1.ipynb`, ..., `ex4.ipynb`) in Jupyter.
- Run the cells sequentially to reproduce the results and visualizations.
- Use ParaView to inspect the exported `.vtu` files.

---

## Requirements

- Python 3.x
- Jupyter Notebook
- numpy, scipy, matplotlib
- porepy
- pygeon

---

## References

- [PyGeoN documentation](https://github.com/compgeo-mox/pygeon)
- [PorePy documentation](https://github.com/pmgbergen/porepy)
- [ParaView](https://www.paraview.org/)
- Standard texts on continuum mechanics and finite element methods

---

*For questions or issues, please contact the course instructor or consult the documentation linked above.*
