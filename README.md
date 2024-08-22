# Sphere-in-Stratified-Fluids
This repository contains the implementation of a numerically assisted mathematical model for a single solid sphere falling through stratified fluids (http://hdl.handle.net/10339/109416). 

There are two versions of the stratified code; one with no boundary layer and one with. Most code that is in these folders has a SaveToPathFunction which creates a directory organized by time automatically. 

The notebook titled Stratified Code _ April 2024.ipynb has no boundary layer, that is you will set the Oseen Kernel and it will run over the entire domain. This code is what was used for the thesis figures as well as the Summer 2024 microplastics in lakes independent study. It runs quickly, and the number of integrations in 𝜃
 can be much larger than 𝜁 and 𝜌. 

The notebook titled NearFieldRadiusCode.ipynb has this control flow. In the control flow code, you set a radius around the sphere where you can pick the kernel in and outside of it. This code has issues when the ANF is close to the sphere radius A, as well as there are issues on the boundary itself. This code has significantly more metrics to track (Forces versus time and position, single entrainment lines, etc). 


- Lane Ellisor - August 2024
