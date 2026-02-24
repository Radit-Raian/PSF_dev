# PSF_dev

**Point Spread Function (PSF) Development Pipeline for Astronomical Imaging**

## Overview

**PSF_dev** is a modular PSF construction and validation pipeline developed for astronomical imaging analysis.  
The pipeline integrates:

- `SExtractor`
- `Photutils`
- `Astropy`

It is designed to:

- Detect point sources from FITS images
- Perform background estimation and subtraction
- Select high-confidence stellar sources
- Mask extended sources
- Construct a clean PSF candidate sample
- Provide diagnostic visualizations

This repository is part of my PSF modeling and image analysis work under astronomical data processing research.
