---
title: "Summary"
description: "Summary"
lead: ""
date: 2020-04-20T11:53:07+02:00
lastmod: 2020-04-20T11:53:07+02:00
draft: false
menu:
  book:
    parent: "4. Collective Neutrino Oscillations"
images: []
weight: 460
toc: true
---


A dense neutrino medium can oscillate collectively because of the neutrino self-interaction potential. When the neutrino flavor conversion probabilities are small, one can apply the linearized flavor stability analysis to find out the regimes where neutrino oscillations begin to develop. I. Izaguirre et al. proposed that the flavor instabilities of a neutrino medium are associated with ``gaps'' between the real dispersion relation curves of the collective modes. In this chapter, I have shown that this association is not valid in general. In particular, I showed that flavor instabilities can exist in three-beam models and in models with continuous but crossed ELN distributions without any gap in the real dispersion relation curves.

I proposed a toy model with two neutrino beams to explore neutrino oscillations with scattered fluxes such as in the supernova model with a neutrino halo. I have developed a relaxation method and a numerical code based on this method to solve this model, and I have validated the numerical code in the scenario where only the neutrino beam and its reflected beam exist.[^code] [^model]

[^code]: The code can be accessed at [github.com/NeuPhysics/neutrino-halo-problem](https://github.com/NeuPhysics/neutrino-halo-problem)
[^model]: In the spirit of numerical methods, I developed a parallelable relaxation method, using C++ and OpenMP. The code is validated using vacuum oscillations and solution to the linearized equation of motion. Both the analytical and numerical results showed that for the single-beam line model is the same as the bipolar model. Thus I can perform linear stability analysis and find out the unstable regions. The reflection indeed may enhance the flavor conversions but I did not find new types of instability using the simple model. Future work should be done to explore the effect of symmetry breaking and multiple emission beams.
