---
layout: default
title: OpenMC
description: OpenMC Monte Carlo Code
---

| [Documentation](https://docs.openmc.org/) | [Discussion Forum](https://openmc.discourse.group/) | [Cross Sections](./cross_sections.html) | [Depletion Chains](./depletion_chains.html) |
        

OpenMC is a community-developed Monte Carlo neutron and photon transport code. It is capable of performing fixed source, k-eigenvalue, and subcritical multiplication calculations on models built using either a constructive solid geometry or CAD representation. A flexible and efficient tally system enables a wide variety of physical quantities to be tallied and analyzed. OpenMC can run in parallel using a hybrid MPI and OpenMP programming model and has been extensively tested on leadership class supercomputers.

One of the unique features of OpenMC is its rich, extensible Python and C/C++ programming interfaces that enable programming pre- and post-processing, multigroup cross section generation, workflow automation, depletion calculations, multiphysics coupling, and the visualization of geometry and tally results. In addition to the core Monte Carlo transport solver and associated APIs, OpenMC includes a Python-based nuclear data interface that enables power users to inspect, modify, and perform various types of nuclear data processing on ENDF, ACE, and OpenMC’s native HDF5 files. To ensure the quality and accuracy of the code over time, a supporting infrastructure has been developed that includes continuous integration testing and automated critical benchmark simulations, cross-code comparisons, and performance testing.