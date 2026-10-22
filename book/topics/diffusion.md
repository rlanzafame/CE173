# Diffusion

This page begins with a brief overview of the diffusion equation, then presents several analytic solutions. There isn't much context for the solutions because the intent is to challenge you to identify the conceptual model that is being solved, then try and relate it to "reality" for any of the example potential fields listed below. 

A generic form of the diffusion equation is typically presented as follows:

$$
\frac{\partial c}{\partial t} = D \nabla^2 c
$$

This equation, often referred to as Fick's second law for the 19th-century scientists work on mass transport, describes how the quantity $c$ changes in time due to spatial variation in potential. Here lower-case $c$ is used to represent the _potential_ field. For our purposes, a potential field is simply a scalar quantity that varies in space, $c(x,y,z)$. While the variable letter, $c$, alludes to concentration, for which Fick's second law was applied, the diffusion equation can be applied to any potential field. Examples include:

- chemical potential: concentration, e.g., $\mathrm{mol/m^3}$ or $\mathrm{kg/m^3}$
- electric potential: voltage, e.g., volts $\mathrm{V}$
- thermal potential: temperature, e.g., Celsius $\mathrm{^\circ C}$ or Kelvin $\mathrm{K}$
- hydraulic potential: total or hydraulic head, e.g., meters $\mathrm{m}$ or feet $\mathrm{ft}$

The diffusion coefficient $D$ characterizes the rate at which the quantity $c$ spreads in space. By inspection, one can see the units of $c$ are irrelevant, as they are present on both sides of the equation, and the units of $D$ are thus related only to length and time: $\mathrm{L^2/T}$. Note that the diffusion coefficient can vary significantly in space and time but is held constant here to enable the derviation of simple analytic solutions.

The operator $\nabla^2$ is the Laplacian, the second order spatial derivative in 3D:

$$
\nabla^2 c = \frac{\partial^2 c}{\partial x^2} + \frac{\partial^2 c}{\partial y^2} + \frac{\partial^2 c}{\partial z^2}
$$

The diffusion equation is a boundary value problem as well as an initial value problem (unlike the Laplace or related steady-state equations). A solution provides a value of the potential in both space and time, $c(x, y, z, t)$ and can be found using numerous analytic approaches, for example:

* Inspection
* Separation of variables
* Fourier transform methods

The focus of this course is to review a few analytic solutions in 1D to understand how the diffusion equation relates to groundwater and contaminant transport problems, then use numerical methods to solve more complex boundary value problems. It is not required to reproduce the derivations of the analytic solutions.

## Storage

Whereas the diffusion equation can be generalized for various potential fields, related properties are analogouse, but different. Recall that a mass balance was used to derive the diffusion equation, such that:

$$
\mathrm{Input} - \mathrm{Output} = \frac{\partial}{\partial t} (\mathrm{Storage})
$$

For the potentials listed above, the storage quantities are:
- chemical potential: mass, $\mathrm{kg/m^3}$
- electric potential: charge, $\mathrm{Coulomb}$
- thermal potential: thermal energy, $\mathrm{J/m^3}$
- hydraulic potential: fluid volume, $\mathrm{m^3/m^3}$

Analytic solutions will use the notation $S$ to refer to the storage quantity, regardless of the specific potential field.

## Dimensional Analysis

Dimensional analysis allows for the comparison of the solution for different applications without worrying about the particular units or physical quantities.

For generic problems it is useful to express the solution for combined values of $Dt$ because the diffusion equation often depends on this product rather than on $D$ and $t$ separately. This leads to the definition of the Fourier number, which is a dimensionless representation of the diffusion process that characterizes the relative importance of diffusion over time. It is defined as:

$$
Fo = \frac{Dt}{L^2}
$$

where $L$ and $t$ are characteristic length and time scales of the system.

Depending on the field of interest, the Fourier number can be used in different ways. Two useful applications are described here. The first is to determine whether the diffusive process has a significant role in transport within the system of interest: a large Fourier number, i.e., $Fo \gg 1$, indicates that diffusion is dominant, whereas a small Fourier number, i.e., $Fo \ll 1$, suggests that diffusion is relatively slow compared to the characteristic time scale of the system.

Another useful application is to evaluate the time required to reach steady state within the system. Taking 1 as a reference value, one can solve for time based on a characteristic length:

$$
t = \frac{L^2}{D}
$$

The characteristic length is problem-specific; if chosen appropriately, the time estimate provides a rough approximation for when the system will reach steady state (i.e., order of magnitude at best).