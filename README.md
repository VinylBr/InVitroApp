# InVitroApp
MATLAB app to simulate in vitro adaptation experiments of M. tuberculosis treated with bedaquiline

## How to install the app
1. Download the raw file
2. Double click the executable file
3. Once installed, the app will appear in apps panel in MATLAB
4. It is recommended to use the App in the fullscreen mode for optimal image re-scaling. 

## Project Overview
We solve a cellular and population level mathematical model that captures bacterial growth, first mutant appearance at its mean waiting times, and drug-mediated killing controlled by intracellular drug levels in each mutant. Here, the model is solved to mimic an in vitro experiment of M. tuberculosis treated with bedaquiline. <br>
Bedaquiline resistance emerges via mutations in _mmpR_ gene that regulates an efflux pump and in _atpE_ that is the drug target <br>
In the simulations, we let one mutation appear in the _mmpR_ and _atpE_ gene. This constrained our model to have four compartments, whic are wild-type (W), MmpR mutant (E), AtpE mutant (T), and a mutant with both _mmpR_ and _atpE_ mutation (ET). <br>

User may choose:
1. Number of passages
2. Bedaquiline concentration in each passage (entered as comma-separated values)
3. Carrying capacity of bacterial population
4. Threshold on bacterial numbers. When total bacterial numbers reach this threshold, the next passage is initiated
5. Inoculum size. This also equals the transfer size that is transferred from one passage to the next 

## Result
Panel 1: Bacterial dynamics of W, E, T, and ET vs time (days) <br>
Panel 2: Trajectory of mutant appearance. Here y-axis denotes the fold-increase in MIC of drug in the strain and x-axis denotes the mean waiting times of a mutant

## Methods used
- MATLAB2022b
- MATLAB AppDesigner
