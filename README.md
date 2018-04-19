# Revisiting Glauber model uncertainties

Compares Npart and Ncoll in Trento to the ALICE Glauber model.

## Usage
```
./generate-events
./make-plots
```

### Comparing Trento and the ALICE Glauber model
![alt text](https://github.com/morelandjs/glauber-attributes/plots/uncertainties.png)

Nucleon participants and binary nucleon-nucleon collisions are used ubiquitiously in heavy-ion physics.
Many experimental measurements rely on precise theoretical knowledge of these
quantities and their model dependent uncertainties.
This repository compares the values of Npart and Ncoll predicted by Trento and the ALICE Glauber model. 
We find that there are large discrepancies between the two models, which arise
from the way nucleon participants are calculated.

Specifically, the Trento model uses a realistic impact-parameter dependent
collision probability Pcoll(b) which is Gaussian, while the ALICE Glauber model
uses a more simplistic "black disk" interaction profile where nucleons collide
with 100% probability if they pass within some maximum distance. 
