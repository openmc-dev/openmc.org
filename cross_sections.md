---
title: 'Cross sections'
license: CC-BY-4.0
github: 'https://github.com/openmc-dev/openmc.org'
---

# Official Data Libraries

The data libraries listed here have been produced by the OpenMC development team and are as complete as possible. HDF5 files are created by first processing source ENDF files into ACE files and then using the [openmc.data](https://docs.openmc.org/en/stable/pythonapi/data.html) Python module to convert ACE data into HDF5. The entire process is automated by the [IncidentNeutron.from_njoy](https://docs.openmc.org/en/stable/pythonapi/generated/openmc.data.IncidentNeutron.html#openmc.data.IncidentNeutron.from_njoy) method which calls [NJOY](http://www.njoy21.io/) under the hood to produce ACE files.

## ENDF/B-VII.1

This library includes incident neutron, photoatomic, thermal scattering, and windowed multipole data. All ACE files were produced using NJOY 2016.68. Incident neutron data is available at six temperatures: 250 K, 293.6 K, 600 K, 900 K, 1200 K, and 2500 K. Note that elastic scattering cross sections are also available at 0 K and and can be used for modeling resonance upscattering in heavy nuclides. Thermal scattering data is available at the tabulated temperatures from the source ENDF files. Windowed multipole data can be used to evaluate temperature-dependent cross sections at run-time.

Downloads: [ENDF/B-VII.1](https://anl.box.com/shared/static/9igk353zpy8fn9ttvtrqgzvw1vtejoz6.xz)

## ENDF/B-VIII.0

This library includes incident neutron, photoatomic, atomic relaxation, and thermal scattering data from ENDF/B-VIII.0. All ACE files were produced using NJOY 2016.68. Incident neutron data is available at six temperatures: 250 K, 293.6 K, 600 K, 900 K, 1200 K, and 2500 K. Thermal scattering data is available at the tabulated temperatures from the source ENDF files.

Downloads: [.tar.xz](https://anl.box.com/shared/static/uhbxlrx7hvxqw27psymfbhi7bx7s6u6a.xz)

## JEFF 3.3

This library includes incident neutron and thermal scattering data from JEFF 3.3. All ACE files were produced using NJOY 2016.68. The photoatomic and atomic relaxation data from ENDF/B-VIII.0 has also been included because JEFF 3.3 does not release its own photoatomic or atomic relaxation sublibraries. Incident neutron data is available at six temperatures: 250 K, 293.6 K, 600 K, 900 K, 1200 K, and 2500 K. Thermal scattering data is available at the tabulated temperatures from the source ENDF files.

Note that the C13 and O17 cannot be processed by NJOY 2016.68 due to a bug in the evaluations. These nuclides have been replaced by data from TENDL-2019 (the original evaluations from JEFF 3.3 were taken from TENDL-2015).

Download: [.tar.xz](https://anl.box.com/shared/static/4jwkvrr9pxlruuihcrgti75zde6g7bum.xz)

# LANL-Based Data Libraries

## ENDF/B-VII.0

This library was produced by converting ACE files generated by the Nuclear Data Team at LANL and distributed with MCNP5/6. Incident neutron data was converted from endf70[a-k] files, thermal scattering data from endf70sab, and incident photon data from the eprdata14 library. Incident neutron data is available at five temperatures: 293.6 K, 600 K, 900 K, 1200 K, and 2500 K. For further information on the source data, please see LANL technical reports LA-UR-08-1999 and LA-UR-08-3628.

Download: [.tar.xz](https://anl.box.com/shared/static/t25g7g6v0emygu50lr2ych1cf6o7454b.xz)

## ENDF/B-VII.1

This library was produced by converting ACE files from the endf71x and ENDF71SaB libraries that were generated by the Nuclear Data Team at LANL and distributed with MCPN5/6. Incident neutron data is available at seven temperatures: 0.1 K, 250 K, 293.6 K, 600 K, 900 K, 1200 K, and 2500 K. Incident photon data converted from the eprdata14 library is also included. For further information on the source data, please see LANL technical reports LA-UR-13-20137 and LA-UR-14-21878.

Download: [.tar.xz](https://anl.box.com/shared/static/d359skd2w6wrm86om2997a1bxgigc8pu.xz)

## ENDF/B-VIII.0

This library was produced by converting ACE files from the Lib80x and ENDF80SaB2 libraries that were generated by the Nuclear Data Team at LANL. Incident neutron data is available at seven temperatures: 0.1 K, 250 K, 293.6 K, 600 K, 900 K, 1200 K, and 2500 K. For more information on the source data, please see LANL technical reports LA-UR-18-24034 and LA-UR-20-24456.

Download: [.tar.xz](https://anl.box.com/shared/static/nd7p4jherolkx4b1rfaw5uqp58nxtstr.xz)

# Other Data Libraries

## JEFF 3.2

This library was produced by converting [ACE files](https://www.oecd-nea.org/dbforms/data/eva/evatapes/jeff_32/) generated by NEA. It includes incident neutron data as well as thermal scattering data for 10 different compounds. Incident neutron data is available at 12 temperatures: 293 K, 300 K, 400 K, 500 K, 600 K, 700 K, 800 K, 900 K, 1000 K, 1200 K, 1500 K, and 2500 K.

Note: This particular library requires that you use HDF5 1.10+ when building OpenMC.

Download: [.tar.xz](https://anl.box.com/shared/static/pb94oxriiipezysu7w4r2qdoufc2epxv.xz)

## JEFF 3.3

This library was produced by converting [ACE files](http://www.oecd-nea.org/dbdata/jeff/jeff33/) generated by NEA. It includes incident neutron data as well as thermal scattering data for 21 different compounds. Incident neutron data is available at 6 temperatures: 293.6 K, 600 K, 900 K, 1200 K, 1500 K, and 1800 K.

Download: [.tar.xz](https://anl.box.com/shared/static/ddetxzp0gv1buk1ev67b8ynik7f268hw.xz)

## FENDL 3.2

This library was produced by converting [ACE files](https://www-nds.iaea.org/fendl_library/websites/fendl32/) generated by IAEA NDS. It includes neutron data for 192 nuclides as well as photoatomic data for 61 elements. Incident neutron data is available at 293.6 K.

Download: [.tar.xz](https://anl.box.com/shared/static/3cb7jetw7tmxaw6nvn77x6c578jnm2ey.xz)
