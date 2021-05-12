# Workshop on Software and Applications of Numerical Nonlinear Algebra

This repository contains the Jupyter notebooks for the

  [Workshop on Software and Applications of Numerical Nonlinear Algebra](https://www.mis.mpg.de/calendar/conferences/2021/sanna2021.html).

Before you download the notebooks:

(1) [download Julia 1.6](https://julialang.org/downloads/)

(2) start a Julia session

(3) go to the package manager by typing `]`

(4) install the following packages:

```julia-repl
pkg> add IJulia
pkg> add HomotopyContinuation
pkg> add https://github.com/PBrdng/Bertini.jl.git
pkg> add https://github.com/PBrdng/PHCpack.git
pkg> add Plots
```

If you want to use Bertini and PHCpack, you have download their binaries and add them to you PATH variable.
