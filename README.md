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
pkg> add ImplicitPlots
```

If you want to use [Bertini](https://bertini.nd.edu) and [PHCpack](http://homepages.math.uic.edu/~jan/PHCpack/phcpack.html), you have download their binaries and add them to your PATH variable.

Once you have downloaded the packages you can solve systems of polynomial equations:
```julia-repl
julia> using HomotopyContinuation
julia> @var x y
julia> f = [x^2 + 2y, y - 2]
julia> result = solve(f)
julia> solutions(result)
2-element Vector{Vector{ComplexF64}}:
 [0.0 - 2.0im, 2.0 + 0.0im]
 [0.0 + 2.0im, 2.0 + 0.0im]
```
More examples can be found in the demo folder.
