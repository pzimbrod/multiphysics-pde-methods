# An Application Driven Method for Assembling Numerical Schemes for the Solution of Complex Multiphysics Problems

This is the source repository for the corresponding preprint.

# Contents

## Article

All sources files for the TeX document can be found in this folder, including references, figures and the source files.

## Benchmarks

This article describes two benchmark cases that are included in this repository.

### Allen Cahn Problem

The Allen Cahn example is implemented using the ```Julia``` programming language.
If you would like to reproduce the results reported, navigate to ```code/Allen-Cahn``` in your terminal. There, you can set up the project using the ```Project.toml``` file with the commands:

```julia
using Pkg
Pkg.activate(".")
Pkg.instantiate()
```

### Advection problem

To run the advection benchmark, you need a working installation of [Firedrake](https://www.firedrakeproject.org/download.html) and its dependencies. Head to the linked website for further installation instructions.

# Citing

This article is currently available as preprint only.
If you use it in your work, please cite as:

```bibtex
@misc{zimbrod2023application,
      title={An Application Driven Method for Assembling Numerical Schemes for the Solution of Complex Multiphysics Problems}, 
      author={Patrick Zimbrod and Michael Fleck and Johannes Schilp},
      year={2023},
      eprint={2309.17055},
      archivePrefix={arXiv},
      primaryClass={math.NA}
}
```

# License

[MIT](https://choosealicense.com/licenses/mit/)
