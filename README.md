# Monte Carlo Neutron Transport Simulation (Python)

This project implements a Monte Carlo simulation of thermal neutron transport through a slab of shielding material. Neutrons are modelled as undergoing random scattering, absorption, transmission, or reflection events based on material properties and interaction probabilities.

## Key features
- Monte Carlo random-walk simulation of neutron trajectories
- Exponential free-path sampling based on macroscopic cross-sections
- Isotropic scattering direction sampling in 3D
- Classification of neutron outcomes (absorbed, transmitted, reflected)
- Uncertainty estimation from repeated simulation runs

## Random number validation
- Tested uniform random number distributions
- Demonstrated isotropic direction sampling on the unit sphere
- Identified spectral artefacts in a linear congruential generator (RANDSSP)

## Material studies
Simulations were performed for different shielding materials (e.g. water, lead, graphite), analysing transmission, absorption, and reflection fractions as a function of slab thickness. Attenuation lengths were estimated via exponential fitting.

## Tech stack
Python, NumPy, Matplotlib

## How to run
```bash
pip install -r requirements.txt
jupyter notebook notebooks/MonteCarloProject.ipynb
