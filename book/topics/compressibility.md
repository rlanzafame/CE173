# Compressibility and Related Properties

See Freeze and Cherry (1979) [Chapter 2.9](https://fc79.gw-project.org/english/chapter-2/#2.9) for background information and typical values.

Compressibility of the soil skeleton, $\alpha$ is defined as the relative change in volume of the soil skeleton per unit change in hydraulic head, which has units of inverse stress (e.g., $\mathrm{m^2N^{-1}}$). Compressibility of water, $\beta$ is defined as the relative change in volume of water per unit change in hydraulic head (same units as $\alpha$).

Specific storage, $S_s$, has units of $\mathrm{L^{-1}}$ and is defined as the volume of water released from a unit volume of aquifer per unit change in hydraulic head:

$$
S_s = \rho_w g (\alpha + n\beta)
$$

where $\rho_w$ is the density of water, $g$ is the acceleration due to gravity, $\alpha$ is the compressibility of the soil skeleton, $\beta$ is the compressibility of water, and $n$ is the porosity of the aquifer.

Storativity is defined for a confined aquifer of uniform thickness $b$ as 

$$
S = S_s b
$$

Transmissivity is also defined for a confined aquifer as the rate at which groundwater can flow through an aquifer of unit width under a unit hydraulic gradient:

$$
T = Kb
$$

where $K$ is the hydraulic conductivity of the aquifer and $b$ is the thickness of the aquifer.

As we have seen in class, the transient groundwater flow equation for a confined aquifer is:

$$
\frac{S}{T} \frac{\partial h}{\partial t} = \frac{\partial^2 h}{\partial x^2}
$$

Or, dropping the $b$ term from $S$ and $T$ and rearranging to the other side:

$$
\frac{\partial h}{\partial t} = \frac{K}{S_s} \frac{\partial^2 h}{\partial x^2}
$$

As such, the ratio $\frac{K}{S_s}$ in the transient groundwater flow equation is the diffusion coefficient for groundwater flow in a confined aquifer.