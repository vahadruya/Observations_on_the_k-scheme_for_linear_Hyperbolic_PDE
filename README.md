# Observations on the k-scheme for linear Hyperbolic PDEs

 A hyperbolic PDE represents the propagation of a wave. The coefficient of the spatial derivative is the speed of the wave propagation in that direction. If a central difference is used in the FV formulation of the hyperbolic wave equation, the spatial derivatives are computed as the fluxes through the control surfaces.

 The objective of this notebook is to analyse the various methods of this spatial discretisation, with the temporal discretisation being explicit. Since this is an advective phenomena, a central differencing with 2nd order accuracy will not suffice to provide good accuracy or a solution with minimal diffusion/dispersion. A general bias for the upwind cells is preferred.

 The various schemes for this spatial discretisation is generalised using the k-scheme.

 For better visualisation of the wave and the effect of this scheme on the wave, a periodic boundary condition is chosen, otherwise the wave will just propagate out of the computational domain
