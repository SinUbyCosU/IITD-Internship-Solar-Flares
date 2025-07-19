IIT Delhi – Summer Research Intern
Department of Physics | May–July 2025
Project: Reconstruction of Umbral Flash and Sunspot Wave Dynamics from AIA and HMI Observations
Reference: Sharma et al. 2017, ApJ, 850:206 – “Direct Observations of Different Sunspot Waves Influenced by Umbral Flashes”

### Objective
To reproduce the spatial and temporal characteristics of umbral flashes and associated sunspot wave structures by replicating Figures 1 and 2 from Sharma et al. (2017), using SDO/AIA and HMI data. Extended the analysis to similar events beyond the original study timeline.
### Blog Post
 Chasing Solar Flares and Losing Sanity: A Summer with Sharma’s Paper:https://medium.com/@yadav23/chasing-solar-flares-and-losing-sanity-a-summer-with-sharmas-paper-8fd650abf475
 
### Technical Summary
Data Acquisition

Retrieved high-cadence UV and magnetogram observations of NOAA AR 11133 from SDO on 2010-12-11, spanning 09:30–10:15 UT.

Channels used:

AIA 1600 Å (24 s cadence, chromosphere),

HMI LOS Magnetograms & Continuum (45 s cadence, photosphere).

Figure 1 (Multi-passband Sunspot Context Panel)

Reconstructed the full active region view across HMI and AIA passbands.

Extracted umbra–penumbra boundaries from HMI continuum, overlaid as black/white contours.

Overplotted coronal fanloop footpoints from AIA 171 Å as blue contours.

Figure 2 (AIA 1600 Å Flash Panel)

Identified and temporally isolated five umbral flashes using brightness spikes in AIA 1600 Å imagery.

Drew a white rectangular box enclosing the flaring region where flashes occurred.

Synchronized frames to match the ~09:46–09:57 UT flash window noted in the paper.

Image Processing & Registration

Applied full-frame derotation using sunpy.image.coalignment tools.

Used WCS-based co-registration to align all AIA and HMI observations spatially and temporally with respect to AIA 171 Å at 09:30:00 UT (as per the paper).

Ensured ~0.6″/pixel consistency across all channels, matching original spatial resolution.

Intensity Normalization

Matched intensity dynamics using AsinhStretch() and PercentileInterval(99.5%) to enhance umbral flash visibility while maintaining background fidelity.

### Project Extension
Applied the same pipeline to 2016 flare events to test repeatability of umbral flash signatures and cross-layer coupling structures.

Aligned preprocessed flare boxes and active region overlays across multiple events to enable comparative spatiotemporal study.

### Tools & Libraries
SunPy, Astropy, NumPy, Matplotlib, FITS, reproject, JSOCClient

 ### Research Significance
Achieved pixel-exact reproducibility of observational figures foundational to multi-height wave propagation studies.

Output ready for integration with:

Time-distance analysis pipelines,

Wavelet power analysis, or

ML-based event sequence modeling (e.g., flare detection/classification from AIA temporal stacks).


