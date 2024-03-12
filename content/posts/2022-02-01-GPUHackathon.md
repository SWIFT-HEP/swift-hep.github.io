---
title: "The simulation Opticks team to participate in the UK Hackathon 2022"
date: 2022-02-01T10:42:55Z
draft: true
start_date: 2022-03-07T10:42:55Z
end_date: 2022-03-09T10:42:55Z
---

<h4> What is the name of your code/application: </h4>
Opticks

<h4>  Application details: </h4>

Optical photon propagation from Cherenkov processes is one of the most time consuming processes of all LHCb simulation. As the problem is embarrasingly parallel and explicitly needed by many particle physics experiments around the world, much work has been undertaken to exploit the RTX cores of modern NVIDIA GPUs to accelerate optical photon simulation and speaking directly to OptiX from the core Geant4 implementation of the detector geometry. This application goes under the name of Opticks and was developed by Simon Blyth (https://simoncblyth.bitbucket.io/opticks/). However, before we became involved, the detector geometries which were involved were relatively simple and unsuited for applications at the Large Hadron Collider. Through use of a simplified example, we have uncovered short-comings in the transformation of the geometry for optical photon processes. We would like to develop a test suite for unit tests for possible geometry implementations to help provide closure tests. In doing so, we hope to also liase with experts to understand the optimal way of geometry transformations to ensure the optimal use of GPU technologies.

<h4> Domain: </h4> 
High energy particle physics, Cherenkov Radiation

<h4> Programming languages: </h4> 
CUDA, C++

<h4> Used libraries: </h4>
 CUDA, RTX, Geant4, ...

<h4>
GPU programming model you intend to use (or currently use) in application: </h4>
CUDA


<h4> Algorithm Motifs: </h4> 
Optical photon propagation off of user-defined surfaces, memory transfer from host to device in efficient manners, random number generation ensuring reproducability and speed.

<h4> 
Current application/code performance? </h4>
The code right now is able to render correctly several complex geometries, and run simple geometries with speedups of 1000x that of nominal Geant4 simulation speeds, however lacks the implementation of all physical properties of solids to be used, and also has issues with the logical subtraction of volumes necessary to make the complex shapes of HEP detectors.

<h4> Software Licenses: </h4>
Apache License, Geant4 Software License, NVIDIA License

<h4> Computing facilities application runs on: </h4>
Any location with cvmfs access, local machines.

<h4>  What do you hope to achieve at the hackathon? </h4>
Understand from experts if there are clear areas for improvement on the geometry transfer from Geant4 to OptiX for GPU acceleration, begin the definition of a unit test suite to automatically ensure capabilities with new releases of underlying software, and to directly consult experts on design choices moving to OptiX 7.


<h4> Is there anything else you'd like to mentino or ask us? </h4>

This work is done through the SWIFT-HEP grant through STFC-UK.
