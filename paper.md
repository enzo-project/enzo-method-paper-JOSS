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
 - name: Andrew Emerick
   orcid: 0000-0003-2807-328X
   affiliation: "1, 10"
 - name: Britton D. Smith
   orcid: 0000-0002-6804-630X
   affiliation: 9
 - name: Cameron B. Hummels
   orcid: 0000-0002-3817-8133
   affiliation: 8
 - name: Lauren Corlies
   orcid: 0000-0002-0646-1540
   affiliation: "5, 6"
 - name: Molly S. Peeples
   orcid: 0000-0003-1455-8788
   affiliation: "5, 7"
 - name: Jason Tumlinson
   orcid: 0000-0002-7982-412X
   affiliation: "5, 7"
 - name: John A. Regan
   orcid: 0000-0001-9072-6427
   affiliation: 11
 - name: David C. Collins
   orcid: 0000-0001-6661-2243 
   affiliation: 12
 - name: Jeffrey S. Oishi
   orcid: 0000-0001-8531-6570
   affiliation: 13
 - name: Iryna Butsky
   orcid: 0000-0003-1257-5007
   affiliation: 14
 - name: Nathan J. Goldbaum
   orcid: 0000-0001-5557-267X
   affiliation: 15
- name: Matthew J. Turk
   orcid: 0000-0002-5294-0198
   affiliation: 15

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
   - name: California Institute of Technology
 index: 8
   - name: University of Edinburgh
 index: 9 
   - name: American Museum of Natural History
 index: 10
   - name: Dublin City University
 index: 11
   - name: Florida State University
 index: 12
   - name: Bates College
 index: 13
   - name: University of Washington in Seattle
 index: 14
   - name: University of Illinois, Urbana-Champaign
 index: 15
  
bibliography: paper.bib
---

# Summary



Enzo [@EnzoGitRepo] is a block-structured adaptive mesh refinement code that is widely used to simulate astrophysical fluid flows (primarily, but not exclusively, cosmological structure formation, star formation, and turbulence).  The code is a community project with dozens of users, and has contributed to hundreds of peer-reviewed publications in astrophysics, physics, and computer science.
The code is Cartesian, can be run in one, two, and three dimensions, and supports a wide variety of physics including (magneto)hydrodynamics, the self-gravity of fluids and particles, cosmological expansion, primordial gas chemistry, optically thin radiative plasma cooling, radiation transport, conduction, and models for star formation, stellar feedback, and the feedback from supermassive black holes.

Enzo's original method paper [@EnzoMethodPaper2014] was published in 2014, and documented Version 2.3.  This paper describes Enzo's most recent public release, Version 2.6 (released on July XX, 2019; see [@EnzoReleaseNotes]).  Since Version 2.3, there have been several new features added to the code:

* Support for the Grackle chemistry and cooling library [@SmithGrackle2017]
* Several new types of adaptive mesh refinement algorithms [@PeeplesFOGGIE2019]
* Cosmic ray pressure, diffusion, and injection [@SalemCRs2014]
* A stochastic forcing module (for driven turbulence calculations) [@SchmidtDrivenTurbulence2009]
* A subgrid-scale turbulence modeling framework [@GreteSGS2017]
* Kinetic supernova feedback [@SimpsonKineticSN2015]
* Magnetic supernova feedback [@ButskyMagneticSN2017]
* An "active particle" framework for complex particle types [@MeeceAGN2017; @ReganRiseSMS2018]
* Fuzzy dark matter evolution [@LiFuzzyDM2019]
* Many new code test problems
* Automated regression testing on GitHub with CircleCI

In addition, there are a much larger number of code enhancements and bug fixes.  A complete listing of new features, enhancements, and bug fixes for all code releases can be found at [@EnzoReleaseNotes].

# Research with Enzo

Enzo is used extensively in the astrophysics research community.  A few recent notable research areas that have benefited from the use of Enzo include:

* Exploration of galaxy formation in the early universe [@SmithPop2Prime2015; @OSheaLuminosity2015; @WiseNature2019] 
* Reionization of the universe [@NormanReion2018]
* High resolution examination of the circumgalactic medium around Milky Way-like galaxies [@SalemCRCGM2016; @PeeplesFOGGIE2019]
* The impact of supermassive black holes on the regulation of galaxy cluster cores [@LiAGN2017; @MeeceAGN2017]
* Astrophysical turbulence [@GreteSGS2017; @KritsukTurb2018]
* Star formation, both in a primordial context and in a Milky Way-type environment [@BurkhartMolCloud2017; @ChiakiPop3to2_2019]
* The interstellar medium and its effect on galaxy behavior [@FujimotoGCM2016; @LiISM2017; @GoldbaumDiskGalaxies2016]
* Supernova deflagration [@HristovSNDeflagration2018]

# Acknowledgments

The development of Enzo has been funded from a wide variety of sources.  The Enzo method paper [@EnzoMethodPaper2014] enumerates support through 2014.  Since then, Enzo development has been funded by 
NASA grants NNX15AP39G (BWO),
NNX17AG23G (JHW), NNX17AF87G (DCC)
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
ACI-1516003 (MLN),
 AST-1616026 (DCC), AAG AST-1715133 (DCC), 
OAC-1810074,
NSF Graduate Research Fellowship DGE 16-44869 (AE),
the Blue Waters Graduate Fellowship, which was supported by NSF  grants No. OCI-0725070 and No. ACI-1238993 and the State of Illinois (IB, AE, FG),
DOE grants ..., 
Michigan State University internal funding (BWO), 
the Los Alamos National Laboratory Institute for Geophysics and Planetary Physics (BWO),
the Marie Skłodowska-Curie Grant – ‘SMARTSTARS’ – grant number
699941 (JAR), 
...

# References
 	