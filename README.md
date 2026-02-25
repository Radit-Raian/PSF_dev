# PSF_dev

**Point Spread Function (PSF) Development Pipeline for Astronomical Imaging**

## Overview

**PSF_dev** is a modular pipeline for constructing high-fidelity Point Spread Functions (PSFs) from astronomical images.  
The pipeline integrates:

- `SExtractor`
- `Photutils`
- `Astropy`

It is designed to:

- Detect point sources from FITS images
- Perform background estimation and subtraction
- Select high-confidence stellar sources
- Mask extended sources
- Construct clean PSF candidate samples
- Provide diagnostic visualizations to assess PSF quality

This pipeline is part of my work in astronomical image analysis, particularly for detecting faint Intracluster Light (ICL) objects and other low-surface-brightness features, where accurate PSF modeling is essential.

To select high-confidence stars for PSF modeling, we use both the `Sextractor` the **Gaia catalog** with the `class_star > 0.99` and  `classprob_dsc_combmod_star > 0.99`. These stars are then matched to the image sources to form the PSF candidate sample. This ensures that only reliable stellar sources are used, improving the accuracy of the PSF and downstream analysis of faint structures like ICL.
