---
title: 'ENZO: An Adaptive Mesh Refinement Code for Astrophysics (Version 2.6) '
tags:
  - adaptive mesh refinement
  - astrophysics
  - galaxy formation 
authors:
 - name: Greg Bryan
   orcid: 
   affiliation: "1, 2"
 - name: Brian O'Shea
   orcid: 0000-0002-2786-0348
   affiliation: 3
 - name: John H. Wise
   orcid: 0000-0003-1173-8847
   affiliation: 4
 - name: Lauren Corlies
   orcid: 0000-0002-0646-1540
   affiliation: "5, 6"
 - name: Molly S. Peeples
   orcid: 0000-0003-1455-8788
   affiliation: "5, 7"
 - name: Jason Tumlinson
   orcid: 0000-0002-7982-412X
   affiliation: "5, 7"

affiliations:
 - name: Columbia University
   index: 1
 - name: Center for Computational Astrophysics
 index: 2
 - name: Michigan State University
 index: 3
 - name: Georgia Institute of Technology
 index: 4
  - name: Johns Hopkins University
 index: 5
  - name: Large Synoptic Survey Telescope
 index: 6
   - name: Space Telescope Science Institute
 index: 7

 
date: 17 July 2019
bibliography: paper.bib
---

# Summary



Enzo [@EnzoGitRepo] is a block-structured adaptive mesh refinement code that is widely used to simulate astrophysical fluid flows (primarily, but not exclusively, cosmological structure formation, star formation, and turbulence).  The code is a community project with dozens of users, and has contributed to hundreds of peer-reviewed publications in astrophysics, physics, and computer science.
The code is Cartesian, can be run in one, two, and three dimensions, and supports a wide variety of physics including (magneto)hydrodynamics, the self-gravity of fluids and particles, cosmological expansion, primordial gas chemistry, optically thin radiative plasma cooling, radiation transport, conduction, and models for star formation, stellar feedback, and the feedback from supermassive black holes.

Enzo's original method paper [@EnzoMethodPaper2014] was published in 2014, and documented Version 2.3.  This paper describes Enzo's most recent public release, Version 2.6 (released on July XX, 2019; see [@EnzoReleaseNotes]).  Since Version 2.3, there have been several new features added to the code:

* Support for the Grackle chemistry and cooling library
* Several new types of adaptive mesh refinement algorithms 
* Cosmic ray pressure, diffusion, and injection
* A stochastic forcing module (for driven turbulence calculations)
* A subgrid-scale turbulence modeling framework
* Kinetic supernova feedback 
* Magnetic supernova feedback
* An "active particle" framework for complex particle types
* Fuzzy dark matter evolution  
* Many new code test problems
* Automated regression testing on GitHub with CircleCI

In addition, there are a much larger number of code enhancements and bug fixes.  A complete listing of new features, enhancements, and bug fixes for all code releases can be found at [@EnzoReleaseNotes].

# Research with Enzo

Enzo is used extensively in the astrophysics research community.  A few recent notable research areas that have benefited from the use of Enzo include:

* Exploration of galaxy formation in the early universe [@SmithPop2Prime2015, @OSheaLuminosity2015, @WiseNature2019] 
* High resolution examination of the circumgalactic medium around Milky Way-like galaxies [@SalemCRCGM2016, @PeeplesFOGGIE2019]
* The impact of supermassive black holes on the regulation of galaxy cluster cores [@LiAGN2017, @MeeceAGN2017]
* Astrophysical turbulence [@GreteSGS2017, @KritsukTurb2018]
* Star formation, both in a primordial context and in a Milky Way-type environment [@BurkhartMolCloud2017, @ChiakiPop3to2_2019]
* ... others ...

# Acknowledgments

The development of Enzo has been funded from a wide variety of sources.  The Enzo method paper [@EnzoMethodPaper2014] enumerates support through 2014.  Since then, Enzo development has been funded by 
NASA grants NNX15AP39G (BWO),
NNX17AG23G (JHW), 
HST-AR-13261.01-A (BWO), 
HST-AR-13895 (JHW), 
HST-AR-14315.001-A (BWO), 
HST-AR-14326 (JHW), 
HST-AR-15012 (LC), 
NSF grants AST-1333360 (JHW), 
AST-1514700 (BWO), 
AST-1517908 (BWO, MSP, LC, JT), 
AST-1614333 (JHW), 
AST-1615848 (BDS, MLN), 
PHY-1430152 (BWO), 
OAC-1835213 (GB, MLN, BWO, JHW),  
DOE grants ..., 
Michigan State University internal funding (BWO), 
the Los Alamos National Laboratory Institute for Geophysics and Planetary Physics (BWO), 
...

# References
