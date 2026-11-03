# Google Colab

A quick guide to getting started with Google Colab.

1. Navigate to https://colab.research.google.com/ 
1. Create a new notebook
1. Activate the Gemini chat
1. Give it the prompt (example copied below)
2. Execute the notebook cells
3. Review results to check that it is correct (both the written Markdown and computed results!).
4. Marvel at what Gemini can do in just a few seconds.


```{admonition} Example Prompt for Gemini
:class: tip

Show me what you can do: set up a few markdown and python code cells that narrate a student through a solution to the 1D diffusion equation for a generic potential C(x) where the boundary condition on the left is C_0 and the condition on the right is C(L)=0. First solve the steady state condition analytically and numerically. Then solve the transient solution analytically and numerically.
```

```{warning}

The output from the prompt above (at least when I ran it---my output is not reproduced on this page) illustrates why it is _very_ important not to skip the **review** step: my prompt gave me the advection-diffusion equation, not the diffusion equation!
```

This produced such nice results that you should pause to appreciate the fact that you just produced something in seconds that took me weeks to accomplish when I was a student. But don't forget: you still have to understand what's happening in the notebook!