# punch-5-meeting

> [!warning]
> **This collection of material is not yet finalized.**

[![DOI](https://zenodo.org/badge/797922406.svg)](https://zenodo.org/doi/10.5281/zenodo.11507132)

Examples from the SOC for the [fifth PUNCH Science Meeting](https://punch.space.swri.edu/punch5meeting.php)

## Data

To access the full set of images go to [https://data.boulder.swri.edu/mhughes/punch_synthetic_data/](https://data.boulder.swri.edu/mhughes/punch_synthetic_data/). 

As data is improved a new version will be released. The first version is in the v1 folder. The second in v2 and so forth.

This data simulates real PUNCH Level 3 data.
It does not include a starfield or F-corona.
The next iteration of this data will include realistic noise.

- L3 - Level 3 total brightness and polarized brightness
    - PAM - PUNCH Level-3 Polarized Low Noise Mosaic – 32 minutes
    - PAN - PUNCH Level-3 Polarized Low Noise NFI Image – 32 minutes
    - PTM - PUNCH Level-3 Polarized Mosaic – 4 minutes
    - PNN - PUNCH Level-3 Polarized NFI Image – 4 minutes

Data are RICE compressed. The calibrated brightness values are stored in the second HDU. An associated placeholder uncertainty array is stored in the third HDU.

Data can be read in with the default astropy.io.fits libraries. 

With the public release of PUNCH Python tools, a more sophisticated data handler capable of reading PUNCH data and bundling the data and WCS information will be available at https://github.com/punch-mission. 
A sample IDL script for reading PUNCH data is under development at https://github.com/punch-mission/PUNCH_IDL_Tools. 

### Description of versions

- v1: the initial version
- v2: fixes WCS misalignment, makes uncertainty more realistic, fixes scaling problem in data

## Getting help

Please open an issue or create a discussion for help with these data and files.
