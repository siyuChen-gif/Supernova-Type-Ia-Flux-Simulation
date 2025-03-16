# SNFluxSim: Supernova Flux Simulation for Type Ia Models

## Overview
This project models the **gamma-ray flux evolution in Type Ia Supernovae (SNe Ia)**, focusing on energy deposition from **Nickel-56 and Cobalt-56 decay**. The simulation implements **core-shell and spherical ejecta models** to analyze how flux propagation changes with different structural assumptions.

## Features
- **Numerical simulation of supernova flux** from radioactive decay over time.
- **Comparison of core-shell and spherical ejecta models**, evaluating gamma-ray escape probabilities.
- **Integration-based flux calculations** using Python and SciPy.
- **Visualization of flux evolution** over a 2500-day period.

## Methodology
1. **Ejecta Expansion:**  
   - The supernova ejecta expands over time as \( a = a_0 + v_0 t \).  
   - Different ejecta structures (core-shell vs. spherical) affect gamma-ray escape.  

2. **Radioactive Decay Modeling:**  
   - \(^{56}Ni \rightarrow ^{56}Co \rightarrow ^{56}Fe \) decay chain.  
   - Flux computed via **integration over ejecta regions**.  

3. **Numerical Integration:**  
   - Uses **quad integration (SciPy)** to compute flux contributions.  
   - Models **attenuation and escape probabilities** for gamma rays.  

4. **Model Comparison:**  
   - **Core-Shell Model:** Differentiates between inner and outer ejecta layers.  
   - **Spherical Model:** Assumes uniform expansion.  

## Installation
Requires Python 3.x and the following libraries:
```bash
pip install numpy scipy matplotlib
