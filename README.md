# PUNCH 5 Science Meeting SOC Materials

[![DOI](https://zenodo.org/badge/797922406.svg)](https://zenodo.org/doi/10.5281/zenodo.11507132)

Examples from the SOC for the [fifth PUNCH Science Meeting](https://punch.space.swri.edu/punch5meeting.php)

## What's here?

This repository includes the following materials:

- *slides.pdf*: slides from Chris Lowder that were presented at the meeting
- *guide.ipynb*: a notebook that explains how to utilize PUNCH data
- *requirements.txt*: the Python packages used by the notebook
- *example_data/*: a few files to explore the data with
- *LICENSE*: a license for using these materials

## Getting started

0. Make sure you have Python 3.10 or later installed.
1. Clone this repo.
2. Install the packages with `pip install -r requirements.txt`. We encourage doing this in a clean virtual environment. [This guide](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/) will help you do this.
3. Open the `guide.ipynb` in your preferred Jupyter environment and follow along.

### What if I use IDL?

A sample IDL script for reading PUNCH data is under development at https://github.com/punch-mission/PUNCH_IDL_Tools. You may find the `guide.ipynb` helpful to learn about how the data is structured, but we do not have a corresponding IDL tutorial.

## What are the `example_data`?

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

### How do I get more data?

To access the full set of images go to [https://data.boulder.swri.edu/mhughes/punch_synthetic_data/](https://data.boulder.swri.edu/mhughes/punch_synthetic_data/).

As data is improved a new version will be released. The first version is in the v1 folder. The second in v2 and so forth.

- v1: the initial version
- v2: fixes WCS misalignment, makes uncertainty more realistic, fixes scaling problem in data

This demo uses `v2` files.

## Getting help

Please open an issue or create a discussion for help with these data and files.
