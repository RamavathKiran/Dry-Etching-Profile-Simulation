# Dry-Etching-Profile-Simulation 
# Dry Etching Profile Simulation

This project simulates the evolution of etch profiles in microfabrication using dry etching techniques, comparing anisotropic and isotropic etch processes.

## Project Overview

The simulation demonstrates:
- **Anisotropic dry etching**: Material is etched primarily in the vertical direction
- **Isotropic dry etching**: Material is removed equally in all directions

The implementation uses MATLAB to generate visual profiles over multiple etch steps and creates animations to visualize trench evolution.

## Files Included

- `anisotropic_etching.m` - MATLAB script for anisotropic etching simulation
- `isotropic_etching.m` - MATLAB script for isotropic etching simulation
- `anisotropic_etching.mp4` - Animation of anisotropic etching process
- `isotropic_etching.mp4` - Animation of isotropic etching process
- `IISC_Simulation.pdf` - Project report with detailed explanation
- `README.md` - This file

## Simulation Methodology

The simulation uses a 2D grid representation where:
- `0` represents etched area (air/vacuum)
- `1` represents material (e.g., silicon)
- `2` represents mask (photoresist/hardmask)

A mask opening is created in the center of the top row, and the etching process evolves over 90 time steps.

## Results

### Anisotropic Etching
- Creates narrow trenches with vertical sidewalls
- No lateral undercut observed
- Etching occurs only in the vertical direction

### Isotropic Etching
- Creates rounded sidewalls with visible undercutting
- Etching spreads laterally beneath the mask
- Matches real-world isotropic behavior

## How to Run

1. Ensure MATLAB is installed on your system
2. Clone this repository
3. Run either script:
   - `anisotropic_etching.m` for anisotropic etching simulation
   - `isotropic_etching.m` for isotropic etching simulation
4. The scripts will generate animations showing the etch profile evolution

## Dependencies

- MATLAB (tested with R2020a or later)
- MATLAB Image Processing Toolbox (for video creation)

## Contributors

- Rajeshwar Raj Singh
- Rakshita MB
- Ralsangkhum Ralsun
- Ramavath Kiran

Group Number 66

## License

This project is for educational purposes as part of academic coursework.
