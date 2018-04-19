# Revisiting Glauber model uncertainties

Compares Npart and Ncoll in Trento to the ALICE Glauber model.

## Usage
```
./generate-events
./make-plots
```

## Description of figures

The following documentation describes each figure in the `plots` directory.

## Nucleon-nucleon collision profile
![alt text](https://github.com/morelandjs/glauber-attributes/blob/master/plots/collision_profile.png)

Nucleon participants and binary nucleon-nucleon collisions are attributes which are used ubiquitiously in heavy-ion physics.
Many experimental measurements rely on precise theoretical knowledge of these
quantities and their model dependent uncertainties.
This repository compares the values of Npart and Ncoll predicted by Trento and the ALICE Glauber model. 
We find that there are large discrepancies between the two models, which arise
from the way nucleon participants are calculated.

Specifically, the Trento model uses a realistic impact-parameter dependent
collision probability Pcoll(b) which is Gaussian (pictured above), while the ALICE Glauber model uses a more simplistic "black disk" interaction profile (black line) where nucleons collide with 100% probability if they pass within some maximum distance.
Although *both* these interaction profiles reproduce the correct proton-proton
inelastic cross section, they lead to significantly different values for Npart
and Ncoll as shown below.

## Comparing Trento and the ALICE Glauber model
![alt text](https://github.com/morelandjs/glauber-attributes/blob/master/plots/uncertainties.png)

This figure compares the values of Npart and Ncoll predicted by Trento and the
ALICE Glauber model.
