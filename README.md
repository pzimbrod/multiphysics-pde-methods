# An Application Driven Method for Assembling Numerical Schemes for the Solution of Complex Multiphysics Problems

This is the source repository for the corresponding article (including the original preprint) published in MDPI Applied System Innovation.

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

If you use it in your work, please cite as:

```bibtex
@Article{asi7030035,
AUTHOR = {Zimbrod, Patrick and Fleck, Michael and Schilp, Johannes},
TITLE = {An Application-Driven Method for Assembling Numerical Schemes for the Solution of Complex Multiphysics Problems},
JOURNAL = {Applied System Innovation},
VOLUME = {7},
YEAR = {2024},
NUMBER = {3},
ARTICLE-NUMBER = {35},
URL = {https://www.mdpi.com/2571-5577/7/3/35},
ISSN = {2571-5577},
ABSTRACT = {Within recent years, considerable progress has been made regarding high-performance solvers for partial differential equations (PDEs), yielding potential gains in efficiency compared to industry standard tools. However, the latter largely remains the status quo for scientists and engineers focusing on applying simulation tools to specific problems in practice. We attribute this growing technical gap to the increasing complexity and knowledge required to pick and assemble state-of-the-art methods. Thus, with this work, we initiate an effort to build a common taxonomy for the most popular grid-based approximation schemes to draw comparisons regarding accuracy and computational efficiency. We then build upon this foundation and introduce a method to systematically guide an application expert through classifying a given PDE problem setting and identifying a suitable numerical scheme. Great care is taken to ensure that making a choice this way is unambiguous, i.e., the goal is to obtain a clear and reproducible recommendation. Our method not only helps to identify and assemble suitable schemes but enables the unique combination of multiple methods on a per-field basis. We demonstrate this process and its effectiveness using different model problems, each comparing the resulting numerical scheme from our method with the next best choice. For both the Allen–Cahn and advection equations, we show that substantial computational gains can be attained for the recommended numerical methods regarding accuracy and efficiency. Lastly, we outline how one can systematically analyze and classify a coupled multiphysics problem of considerable complexity with six different unknown quantities, yielding an efficient, mixed discretization that in configuration compares well to high-performance implementations from the literature.},
DOI = {10.3390/asi7030035}
}
```

# License

[MIT](https://choosealicense.com/licenses/mit/)
