# Numerical Analysis

This chapter provides a _very_ broad overview of numerical analysis techniques for solving groundwater flow equations. We will consider diffusion, advection and the diffusion-advection equations. As the diffusion equation solves the transient groudnwater flow equations, we can run our numerical simulation for long times to approximate steady-state solutions.

A complete treatment of numerical analysis is well beyond the scope of our course. 

Topics to be aware of include:

- Discretization methods (finite difference, finite element, finite volume)
- Stability and convergence of numerical schemes
- Time-stepping methods for transient simulations
- Handling boundary and initial conditions
- Error analysis and estimation



Robert's Simplified Approach

1. Identify your problem in real life. This includes conceptual diagrams, sketching physical limits of your problem,boundary conditions, evaluation of available data.
2. Itentify your model: PDE's that are appropriate, key assumptions, simplifying BC's, etc.
3. Pick a method:
   1. PhD approach: theory, discretization, implementation, new code.
   2. Consultant approach: pick an existing software.
   3. An approach more common in the future? Use AI to write code and applications.
4. Calibrate, verify and validate your model against the data.
5. Use the model to make preductions, inform decisions, etc. Often this includes a sesitivity analysis.
6. Document the results and, _perhaps more importantly,_ the model and analysis approach.