# FourierSeries.jl

This is a Julia package on the analysis and synthesis of Fourier series.
The determination of Fourier coefficients is based on real value data.
The Fourier coefficients may be calculated either real of complex. The module FourierSeries.jl is tested with Julia 0.6.2.

The non-official package FourierSeries.jl can be installed by (has to be done only once):

```julia
Pkg.clone("git://github.com/christiankral/FourierSeries.jl.git")
```

In order to update to the actual version of GitHub use:

```julia
Pkg.update("FourierSeries")
```

The module FourierSeries.jl has to be loaded by `using FourierSeries`.

**Note:**  After updating to a newer version of FourierSeries.jl, the module can be reloaded without exiting the session by applying `reload("FourierSeries")`.

# Analysis Functions

- `fourierSeriesStepReal(t,u,hMax)` This function determines the real value Fourier coefficients of a piecewise constant time domain function u(t)

- `fourierSeriesSampledReal(t,u,hMax)` This function determines the real value Fourier coefficients of a sampled time domain function u(t)

# Synthesis Functions

- `fourierSeriesSynthesisReal(f,a,b,hMax,N)` This function synthesizes the time domain function from the frequency vector and real value Fourier coefficients `a` and `b`
