# General Solution

The general, steady-state analytical solution for the head distribution due to pumping from a well, $i$,  at a location $x_i,y_i$ in a 2D flow domain is given by:

$$
ℎ(𝑥,𝑦)=𝑖(𝑥𝑐𝑜𝑠𝜃+𝑦𝑠𝑖𝑛𝜃)+\frac{1}{{4\pi}𝐾𝑏} \sum_{𝑖=1}^{𝑛}𝑄_𝑖 ln\sqrt{[(x-x_i)^2+ (y-y_i)^2]}+𝑐
$$

where c is the offset based on the initial boundary head and

$$
ln r= ln \sqrt{(x-x_i)^2+(y-y_i)^2}
$$

The equivalent solution for the head distribution in an unconfined aquifer is then given by

$$
ℎ^2(𝑥,𝑦)=𝑖(𝑥𝑐𝑜𝑠𝜃+𝑦𝑠𝑖𝑛𝜃)+\frac{1}{{2\pi}𝐾} \sum_{𝑖=1}^{𝑛}𝑄_𝑖 ln\sqrt{[(x-x_i)^2+ (y-y_i)^2]}+𝑐
$$

The picture illustrates a solution for a single well in a uniform flow field with stream lines (orthogonal to flow lines) and equipotential lines. The code to produce this solution is included in the next section.

```{figure} ./diagram/example.jpg
---
scale:45%
align: center
---
Example Zone of Capture in a Uniform Flow Field
```
