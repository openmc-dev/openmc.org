---
layout: default
title: Cross Sections
description: Download h5 cross sections for use in OpenMC
---

#Depletion Chains

In order to perform depletion analysis using [the OpenMC depletion module](https://docs.openmc.org/en/latest/pythonapi/deplete.html), a representation of the depletion chain must be presented. This chain describes transmutation and decay channels causing isotopes to evolve over time. XML-representations of these depletion chains can be built using evaluated nuclear data libraries. OpenMC provides [functions](https://docs.openmc.org/en/latest/pythonapi/generated/openmc.deplete.Chain.html#openmc.deplete.Chain.from_endf) and scripts to generate these chain files using a collection of neutron interaction, neutron-induced fission, and decay files. Alternatively, three pre-generated chain files are made available using [ENDF/B-VII.1 data distributed with OpenMC](http://openmc.org/official-data-libraries/).

ENDF/B-VII.1 Chain (Thermal Spectrum)

Provided here is a complete depletion chain containing all isotopes with cross sections, neutron-induced fission yield data, and decay data as contained in the ENDF/B-VII.1 libraries distributed with OpenMC. Capture branching ratios are taken to be identical to the [default branching ratios used in the Serpent](http://serpent.vtt.fi/mediawiki/index.php/Default_isomeric_branching_ratios) Monte Carlo code, corresponding to a typical PWR spectrum.

Download:

    for version 0.11 [.xml](https://anl.box.com/shared/static/1ndcrc1j042nkdpfobp5ebsyxghziisc.xml)
    for version 0.12+ [.xml](https://anl.box.com/shared/static/os1u896bwsbopurpgas72bi6aij2zzdc.xml)

ENDF/B-VII.1 Chain (Fast Spectrum)

Provided here is a similar complete depletion chain, but using capture branching ratios that are more representative of a sodium fast reactor (SFR). Branching ratios were computed by tallying total capture reaction rates, capture to ground, and capture to metastable states for specific isotopes. The effective branching ratios were taken to be the ratio of reactions to ground to total number of capture reactions for each isotope.

Download:

    for version 0.11 [.xml](https://anl.box.com/shared/static/bb7sfrrf6pyyoa5zoa2sxiuy7mvn5kza.xml)
    for version 0.12+ [.xml](https://anl.box.com/shared/static/9058zje1gm0ekd93hja542su50pccvj0.xml)

ENDF/B-VIII.0 Chain (Thermal Spectrum)

This is a complete depletion chain generated based on the incident neutron, decay, and neutron fission yield sublibraries from ENDF/B-VIII.0. Capture branching ratios are taken to be identical to the [default branching ratios used in the Serpent](http://serpent.vtt.fi/mediawiki/index.php/Default_isomeric_branching_ratios) Monte Carlo code, corresponding to a typical PWR spectrum.

Download: [.xml](https://anl.box.com/shared/static/nyezmyuofd4eqt6wzd626lqth7wvpprr.xml)
ENDF/B-VIII.0 Chain (Fast Spectrum)

This is a complete depletion chain generated based on the incident neutron, decay, and neutron fission yield sublibraries from ENDF/B-VIII.0. Capture branching ratios used within are representative of a sodium fast reactor (SFR). Branching ratios were computed by tallying total capture reaction rates, capture to ground, and capture to metastable states for specific isotopes. The effective branching ratios were taken to be the ratio of reactions to ground to total number of capture reactions for each isotope.

Download: [.xml](https://anl.box.com/shared/static/x3kp739hr5upmeqpbwx9zk9ep04fnmtg.xml)
Simplified Chain (Thermal Spectrum)

Provided here is a simplified depletion chain using isotopes recommended by Appendix A of Kang Seog Kim, “Specification for the VERA Depletion Benchmark Suite”, CASL-U-2015-1014-000, Rev. 0, ORNL/TM-2016/53, 2016. Te129 has been included, due to its link to I129 production. Capture branching ratios representative of a PWR spectrum are applied to relevant isotopes.

Download:

    for version 0.11 [.xml](https://anl.box.com/shared/static/lv4b1epe8kwfvqtzhaik19outb9s4vta.xml)
    for version 0.12+ [.xml](https://anl.box.com/shared/static/3nvnasacm2b56716oh5hyndxdyauh5gs.xml)

Simplified Chain (Fast Spectrum)

Provided here is a simplified depletion chain using isotopes recommended by Appendix A of Kang Seog Kim, [“Specification for the VERA Depletion Benchmark Suite”](https://doi.org/10.2172/1256820), CASL-U-2015-1014-000, Rev. 0, ORNL/TM-2016/53, 2016. Te129 has been included, due to its link to I129 production. Capture branching ratios representative of an SFR spectrum are applied to relevant isotopes.

Download:

    for version 0.11 [.xml](https://anl.box.com/shared/static/4j27ca0l112krbw9nldj195bqik9qgvn.xml)
    for version 0.12+ [.xml](https://anl.box.com/shared/static/9fqbq87j0tx4m6vfl06pl4ccc0hwamg9.xml)

Capture Branching Ratios

Below are links to tabulated representations of the capture branching ratios computed using PWR and SFR spectra. The PWR branching ratios are taken from the Serpent Wiki. The SFR branching ratios are computed by computing one group total capture, capture to ground, and capture to metastable states in an SFR assembly.

    [PWR Spectrum Capture Branching Ratios](http://openmc.org/pwr-spectrum-capture-branching-ratios/)
    [SFR Spectrum Capture Branching Ratios](http://openmc.org/sfr-spectrum-capture-branching-ratios/)
