# Energy-Based Gravitational Dominance in the Solar System

A computational investigation of gravitational dominance in planetary systems using an energy-based framework combined with Hill-radius scaling.
"Gravitational Dominance in Planetary Systems: An Energy -Based Hill-Radius Scaling Approach"
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.20385542.svg)](https://doi.org/10.5281/zenodo.20385542)


## Author

Ömür Çarboğa  
2026


## Overview

This project explores how gravitational influence varies across planetary systems by comparing the gravitational potentials associated with celestial bodies and the Sun. Distances are normalized using the Hill radius, allowing systems spanning several orders of magnitude in mass to be analyzed within a common framework.

The numerical analysis examines:

- Earth
- Mars
- Jupiter
- Asteroid (101955) Bennu

using Python-based simulations.


## Research Motivation

The Hill radius is widely used in celestial mechanics as a geometric measure of gravitational influence. However, spatial scaling alone does not necessarily describe how gravitational environments behave energetically.

This study investigates whether Hill-radius normalization also produces a common energetic structure across planetary systems.

Instead of evaluating gravitational dominance through force balance, the model compares gravitational potential energies:

S_E = |U_body| / |U_sun|

where:

U = -GM/r

This formulation provides an energy-based perspective on gravitational influence and allows comparison between geometric and energetic descriptions of planetary environments.


## Relation to Previous Work

This study extends a previous force-based investigation completed in March 2026.

### Previous Study (March 2026)

Force-based gravitational dominance:

S_F = F_body / F_sun

The previous work investigated dominance using gravitational force balance and examined how force-based influence varies with Hill-radius scaling.

### Present Study (April 2026)

Energy-based gravitational dominance:

S_E = |U_body| / |U_sun|

The present work reformulates the analysis using gravitational potential energy rather than instantaneous force.

This transition allows investigation of how energetic influence differs from local force dominance and highlights important distinctions between geometric, force-based, and energetic interpretations of gravitational environments.


## Methodology

The simulation:

- Computes Hill radii for each body
- Normalizes distance using R_H
- Evaluates energetic dominance over:

0.01–2 Hill radii

- Detects energetic transition locations using:

S_E = 1

The model uses the approximation:

r << a

allowing the particle–Sun distance to be approximated by the orbital radius of the analyzed body.


## Main Findings

Key results:

- Jupiter exhibits the only energetic dominance transition within the sampled interval.
- Earth and Mars remain below the transition threshold.
- Bennu remains several orders of magnitude below unity.
- Hill-radius normalization provides geometric scaling but does not produce a universal energetic structure.
- The existence of energetic dominance depends strongly on system mass and gravitational potential depth.


## Model Limitations

This model intentionally simplifies gravitational dynamics.

The simulation:

- Does not solve the Restricted Three-Body Problem
- Does not perform N-body integrations
- Neglects perturbations from additional bodies
- Uses a static energetic framework
- Does not model long-term orbital evolution

Therefore:

S_E = 1

should be interpreted as an approximate indicator of energetic dominance rather than a precise dynamical stability boundary.


## Requirements

Required Python libraries:

```bash
pip install numpy matplotlib pandas
```


## Citation

If you use this work, please cite:

Ömür Çarboğa
"Gravitational Dominance in Planetary Systems: An Energy-Based Hill-Radius Scaling Approach"
2026

Related work:

Ömür Çarboğa
"Gravitational Dominance in Planetary Systems: An Force-Based Hill-Radius Scaling Approach"
2026
