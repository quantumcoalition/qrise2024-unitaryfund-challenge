# QRISE 2024 Mitiq Challenge: Stacking Quantum Error Mitigation Techniques

### Summary

In this research challenge, you will explore the efficacy of stacking multiple quantum error mitigation techniques leveraging the Mitiq Python toolkit. The goal is to compare different combinations of error mitigation strategies in simulation to achieve the lowest possible error rate.

### Background

Quantum computers hold immense potential for solving complex problems, but their practical utility is hindered by their susceptibility to errors. Mitigating these errors is crucial for realizing the full capabilities of quantum computers. This challenge aims to find effective methods of reducing noise by means of combining multiple Quantum Error Mitigation (QEM) techniques. QEM is a field of research that aims to find ways to increase the accuracy of quantum computers without the full machinery needed to implement quantum error correction. A plethora of QEM techniques have been proposed and studied over the past ~7 years such as [Zero-Noise Extrapolation](https://mitiq.readthedocs.io/en/stable/guide/zne.html) [2], [Probabilistic Error Cancellation](https://mitiq.readthedocs.io/en/stable/guide/pec.html), [Quantum Subspace Expansion](https://mitiq.readthedocs.io/en/stable/guide/qse.html), [Dynamical Decoupling](https://mitiq.readthedocs.io/en/stable/guide/ddd.html), etc, yet the capabilities of these techniques have not been thoroughly tested and explored in conjunction with each other (see [2-3] for research in this direction, and [4] for testing on hardware). Recent work in Layerwise Richardson Extrapolation [5] is very exciting and currently being added to Mitiq. Adapting some of the available [research code](https://github.com/unitaryfund/research/tree/main/lre) could be used to find increased performance improvements when coupling with other techniques [[related tutorial](https://mitiq.readthedocs.io/en/stable/examples/layerwise-folding.html)].

The python toolkit Mitiq contains many of the popular error mitigation techniques. Various QEM “stacks” (i.e. combinations of techniques) should be simulated on a suite of benchmark circuits (e.g. [randomized benchmarking](https://mitiq.readthedocs.io/en/stable/apidoc.html#mitiq.benchmarks.randomized_benchmarking.generate_rb_circuits) circuits, [mirror](https://mitiq.readthedocs.io/en/stable/apidoc.html#mitiq.benchmarks.mirror_circuits.generate_mirror_circuit) circuits, [GHZ](https://mitiq.readthedocs.io/en/stable/apidoc.html#mitiq.benchmarks.ghz_circuits.generate_ghz_circuit) circuits, [W-state](https://mitiq.readthedocs.io/en/stable/apidoc.html#mitiq.benchmarks.ghz_circuits.generate_ghz_circuit) circuits, etc), with different noise models to get a sense of how each stack performs in a wide variety of situations. We encourage participants to run these on other circuits that are of interest to them!

### Sources

1. [arxiv:2005.10921](https://arxiv.org/abs/2005.10921)
2. [arXiv:2301.02690](https://arxiv.org/abs/2301.02690)
3. [arXiv:2204.06056](https://arxiv.org/abs/2204.06056)
4. [arXiv:2210.07194](https://arxiv.org/abs/2210.07194)
5. [arXiv:2402.04000](https://arxiv.org/abs/2402.04000)

Submission format: Tutorial/notebook demonstrating the use of multiple techniques in conjunction. Opening new issues on Mitiq is encouraged as participants use, and encounter issues with, Mitiq. Adding a tutorial to Mitiq’s documentation demonstrating a performance gain from stacking QEM techniques.
