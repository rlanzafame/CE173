# Numerical Analysis

This chapter provides a _very_ broad overview of numerical analysis techniques for solving groundwater flow equations. We will primarily focus on the diffusion equation. As the diffusion equation solves the transient groudnwater flow equations, we can run our numerical simulation for long times to approximate steady-state solutions.

A complete treatment of numerical analysis is well beyond the scope of our course. Topics to be aware of include:

- Discretization methods (finite difference, finite element, finite volume)
- Stability and convergence of numerical schemes
- Time-stepping methods for transient simulations
- Handling of boundary conditions and initial conditions
- Error analysis and estimation

## Additional Resources

If you intend to dive deeper into numerical analysis, it is well worth your time to take a dedicated course on the subject: at UC Berkeley it is Math 128A. There are also a number of online resources available. Note, however, that this is a topic that benefits greatly from dedicated practice, both analytical and numerical---reading is simply not enough for most students.

MUDE (Modeling, Uncertainty and Data for Engineers) was a course I was involved with when teaching in the Netherlands; we created a _lot_ of useful open source online resources, most of which can be found in an online textbook.

[Fundamental topics in numerical analysis](https://mude.citg.tudelft.nl/book/2025/numerical_methods/overview.html) covers numerical differentiation and integration methods (in time and space), stability and error analysis.

The [Finite Difference Method](https://mude.citg.tudelft.nl/book/2025/numerical_methods_for_PDEs/overview.html) focuses on shallow water wave equations, but shows general principles for several types of PDE's.

The [Finite Volume Method](https://mude.citg.tudelft.nl/book/2024/fvm/fvm.html) is described in an older version of the same book from 2024. There is also a [concise overview page covering a variety of conservation laws and PDE operators](https://mude.citg.tudelft.nl/book/2024/fvm/getting_started_new.html).

## Robert's Simplified Approach to Numerical Modeling

Most engineers and scientists these days do not write programs themselves to solve complex problems; instead, they rely on existing software. This is especially true if you work in the consulting industry. Here is a brief list of the key modeling steps that should be carried out when using software; note that the time and attention paid to each step can vary significantly depending on available data, project scope and standards of practice in the relevant field.

Perhaps more importantly at the moment: you will use this list to carry out the final project for this course.

1. **Identify your problem in real life.** This includes making conceptual diagrams, sketching physical limits of your problem, evaluation of available data.
2. **Itentify your model:.** At minimum, identify the PDE's that are appropriate, key assumptions, simplifying BC's, etc.
3. **Pick a method.** 
   1. PhD approach: theory, discretization, implementation, new code.
   2. Consultant approach: pick an existing software. Make sure you review the documentation to confirm that it can solve the problem you are interested in.
   3. An approach more common in the future? Use AI tools to write custom code and applications.
4. Calibrate, verify and validate your model against the data.
5. Use the model to make predictions, inform decisions, etc. Often this includes a sensitivity analysis.
6. Document results and, _perhaps more importantly,_ the model and analysis approach.