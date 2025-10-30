# MODELING AND SIMULATION OF FAULT STABILITY IN SUBSURFACE FLUID INJECTION

## Course Overview

This course introduces the mathematical and numerical modeling of fault stability in subsurface settings influenced by fluid injection and production. The program begins with porous media flow governed by Darcy's law, followed by linear elasticity for rock deformation. These concepts are combined through Biot's poroelastic framework to describe coupled hydro-mechanical effects that alter stresses near geological faults. The course then addresses contact mechanics and the criteria that control the onset of fault slip, highlighting their relevance to pre-seismic behavior. Numerical strategies, including decoupling approaches and computational methods for stability assessment, are presented alongside illustrative examples.

The course is hands-on and computational, with a strong emphasis on the implementation and analysis of numerical methods for PDEs relevant to fault mechanics and subsurface fluid flow. Each laboratory is designed to reinforce theoretical concepts through practical coding exercises and realistic scenarios, providing insight into solution techniques and physical interpretations.

## Laboratory Structure and Content

The laboratory component is organized into a series of Jupyter notebooks, each focusing on a specific mathematical model or numerical technique. The labs are designed to be self-contained and build progressively in complexity, covering:

- Darcy's equation for porous media flow
- Finite element and finite volume discretizations for flow problems
- Linear elasticity equations and stress/strain analysis
- Poroelastic equations (Biot's theory) for coupled hydro-mechanical problems
- Decoupling strategies and iterative splitting solvers
- Contact mechanics and fault slip criteria
- Stability assessment methods for fault activation
- Post-processing and visualization with ParaView

### Example Laboratory Topics

- **Lab 1**: Darcy's equation (flow in porous media, boundary conditions, discretization methods)
- **Lab 2**: Linear elasticity (stress and displacement fields, constitutive relations)
- **Lab 3**: Biot's poroelastic equations (coupled flow and deformation, fixed-strain and fixed-stress methods)
- **Lab 4**: Fault stability analysis (contact mechanics, Coulomb failure criterion, slip tendency)

Each lab includes:

- A mathematical introduction and problem statement
- Step-by-step code for grid generation, discretization, and solution
- Implementation of boundary and initial conditions
- Assembly and solution of linear systems
- Post-processing: computation of derived quantities (e.g., stress, pressure, displacement) and export for visualization
- Consistency checks and validation

## Getting Started

### Installation for Linux

The package requires Python >= 3.13

Many functionalities depend on [PorePy](https://github.com/pmgbergen/porepy) and [PyGeoN](https://github.com/compgeo-mox/pygeon), so these packages will be installed. To install all the dependencies:

```bash
pip install -e .
```

### Running the Laboratories

1. Clone the repository and install dependencies as above.
2. Open the desired lab notebook (e.g., `lab/lab1/ex1.ipynb`) in Jupyter.
3. Follow the instructions and run the cells sequentially.
4. Use ParaView or similar tools to visualize exported `.vtu` files.

## Learning Outcomes

By the end of the course and laboratory sessions, students will:

- Understand the mathematical formulation of Darcy's equation, linear elasticity, and Biot's poroelastic equations.
- Be able to discretize and solve these equations using modern numerical methods.
- Gain practical experience with Python-based scientific computing tools for subsurface modeling.
- Analyze coupled hydro-mechanical effects and their impact on stress changes near faults.
- Understand contact mechanics and the criteria that govern fault slip initiation.
- Develop skills in stability assessment for fault activation in subsurface fluid injection scenarios.
- Analyze and interpret simulation results, including stress, displacement, pressure, and flux fields.
- Develop skills in debugging, validation, and scientific visualization.

## Issues

Create an [issue](https://github.com/compgeo-mox/lec_massif/issues).

## License

See [license](./LICENSE).

## References and Further Reading

- [PyGeoN documentation](https://github.com/compgeo-mox/pygeon)
- [PorePy documentation](https://github.com/pmgbergen/porepy)
- [ParaView](https://www.paraview.org/)
- Standard texts on poroelasticity, fault mechanics, and numerical methods for coupled problems

For questions or issues, please contact the course instructor or consult the documentation linked above.