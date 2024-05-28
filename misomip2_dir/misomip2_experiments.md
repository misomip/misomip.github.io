---
layout: post
title: MISOMIP2 Experiments
date: 02-11-2023
---

The MISOMIP2 experiments were designed with two broad objectives in mind. First, to test and intercompare the fidelity of ice-shelf--ocean models and ice-sheet--ocean models over the observational period, and second, to assess the sensitivity of models to a plausible change in the shape of the ice-shelf cavities and to a large perturbation in the atmospheric forcing. In all the following, _A_ stands for Amundsen, and _W_ for Weddell.

* **OceanA-hind & OceanW-hind** experiments are designed to compare stand-alone ocean model simulations with static ice shelves and present-day atmospheric forcing to a common set of ocean observations that are relevant to Antarctic ice shelves, to analyse multi-model sensitivity to external drivers, and to potentially identify clusters of models with a similar behaviour for specific modelling choices. 

* **OceanA-warm & OceanW-warm** experiments are designed to compare the response of simulated melt rates to a transition to very warm ocean conditions, in response to a rapid modification of the atmospheric forcing. The model configuration is otherwise identical to the OceanA-hind and OceanW-hind experiments. All models will apply a strong atmospheric perturbation representative of an abrupt shift to a warmer climate in the form of a prescribed anomaly to be added to the present-day forcing used in the OceanA-hind & OceanW-hind experiments. For regional models with open ocean boundaries, an additional temperature and salinity anomaly is provided for the boundaries to represent the ocean warming outside the domain.

* **OceanA-ctrl & OceanW-ctrl** experiments are extensions of OceanA-hind & OceanW-hind and forced by present-day atmospheric conditions to be used as a control for the perturbation experiments.

* **OceanA-Pgeom, OceanA-Fgeom, OceanW-Pgeom, OceanW-Fgeom** experiments are designed to compare the response of simulated melt rates in stand-alone ocean models to an imposed modification of the ice-shelf geometry. Two distinct geometries for the Amundsen Sea and Filchner-Ronne cavities are provided: one that represents the present-day state of the ice sheet (OceanA-Pgeom and OceanW-Pgeom experiments), and one hypothetical future state (OceanA-Fgeom and OceanW-Fgeom experiments). The atmospheric forcing remains unchanged between these experiments. The difference between Ocean\*-Pgeom and Ocean\*-hind experiments is that in the former, the present-day geometry of the ice shelves is prescribed and provided as part of the MIPkit, whereas in the latter the user is free to choose a present-day ice-sheet geometry as part of the CAYA approach.

* **IceOceanA-hind & IceOceanW-hind** experiments are similar to OceanA-hind & OceanW-hind focusing on present-day conditions, but with coupled ice-sheet--ocean models (including intermediate-complexity coupling through parameterisations). Here we aim to compare the simulated ice and ocean evolution to recent observations. We will also attempt to estimate the bias reduction (if any) that such coupled models attain compared to standalone ocean models.

* **IceOceanA-warm & IceOceanW-warm** experiments are designed to compare the response of the coupled system to the same idealised very warm perturbation as for OceanA-warm & OceanW-warm.

* **IceOceanA-ctrl & IceOceanW-ctrl** experiments are extensions of IceOceanA-hind & IceOceanW-hind over several present-day cycles, to be used as control for the perturbation experiments. This is used to account for possible drifts in the simulation.
