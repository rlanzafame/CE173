# Zone of Capture Analysis

Zone of capture refers to the water in an aquifer that is "captured" by one or more wells. Here a solution is presented to compute and visualize this zone in 2D plan view (i.e., above) and as a 3D interactive surface.

_This section is based on content and code by Nicholas Sitar._

The analysis assumes steady-state flow in a confined aquifer, although it can be applied to unconfined flow with a bit of judgement as long as the gradients are not too large. The transmissivity, T $[L^2/T]$, of a tabular aquifer is computed as $T=Kb$, where $K$ is the hydraulic conductivity and $b$ is the thickness of the aquifer. The gradient, $i$, determines how fast the water moves through the aquifer and the zone of capture is the portion of the aquifer in which the water is captured by a well pumping at a rate $Q$. If the width of the zone of capture is denoted as $2y_L$ then then

$$
Q=iKb2y_L \quad [L^3/T]
$$

and the width of the zone of capture is

$$
2y_L=\frac{Q}{iKb}
$$

The diagram below shows the concept. Note that in the diagram the $x$-axis is parallel to the direction of flow and $y$-axis is orthogonal to the direction of flow. This convention makes the solution very simple for a problem with a single well, as shown in the Figure. 
```{figure} ./capture/diagram.jpg
---
scale:45%
align: center
---
Zone of Capture Illustration
```
The final item is the stagnation point, which is the point at which the gradient is exactly zero downgradient from the well as shown in the figure. The expression to compute the distance of this point downgradient is:

$$
x_{L}=-\frac{Q}{2{\pi}Kbi}
$$

The position of the flow line marking the divide between the flow bypassing the well and the flow line captured by the well is given by

$$
y=-x\tan\left(\frac{2{\pi}Kbi}{Q}\right)
$$
