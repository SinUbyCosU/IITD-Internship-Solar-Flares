IIT Delhi – Summer Research Intern
Department of Physics | May–July 2025
Project: UV Flash Analysis of Solar Flares using AIA 1600 Å and HMI Data
Based on: Sharma et al., ApJ 850:206 (2017)

###What I Built###

AIA-HMI Derotation + Alignment:
Implemented WCS-accurate derotation and temporal co-alignment of AIA 1600 Å images with corresponding HMI continuum and LOS magnetogram data using SunPy, Astropy, and JSOC.
 Blog Write-Up
Chasing Solar Flares and Losing Sanity: A Summer with Sharma’s Paper
 Read on Medium:https://medium.com/@yadav23/chasing-solar-flares-and-losing-sanity-a-summer-with-sharmas-paper-8fd650abf475
 
###Arcsecond-level Region Selection:###
Used SkyCoord and full WCS transformation to crop flaring subregions with high precision, matching annotated ROIs in Sharma et al. (e.g., the white flash box in Figure 2).

Photometric & Visual Reproduction:
Reconstructed flare panels using AsinhStretch and PercentileInterval(99.5) normalization to match brightness gradients and flash contrast in the original AIA images.

Annotation Layer Rendering:
Programmatically overlaid umbra–penumbra boundaries, rectangular flash regions, and fan-loop footpoint markers — preserving exact placements as described in the paper.

Cross-Time Event Generalization:
Extended this entire workflow to similar flare events in 2016, exploring consistency in magnetic coupling and UV signatures across time — laying the foundation for a scalable, multi-event analysis pipeline.

### Why It Matters###
This wasn’t just figure replication — it was about rebuilding a scientific workflow from scratch, verifying results, and pushing it forward. It gave me deep exposure to:

Real-world multimodal, spatiotemporal astrophysical data,

Coordinate frame handling and image transformations in WCS-aware systems,

The rigor needed for reproducible science and open data pipelines.

It also opened up an exciting ML direction: encoding sequences of aligned AIA/HMI maps as inputs to temporal neural architectures (like ViTs or ConvLSTMs) for flare detection, classification, or precursors modeling.

###Stack###
Languages & Libraries: Python, SunPy, Astropy, JSOC API, Matplotlib, NumPy

Data: SDO/AIA 1600 Å UV imagery, HMI LOS magnetograms & continuum

Techniques: Image registration, WCS transforms, scientific normalization, data visualization

ML-Ready Outputs: Cropped, aligned, intensity-normalized sequences for time-series modeling


