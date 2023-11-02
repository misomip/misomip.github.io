---
layout: page
title: MIPkit-Perturbations
date: 02-11-2023
---

### Atmospheric forcing perturbation (A1vw, W1vw)

```
Atm_*_anomaly_MISOMIP2.nc
```

These data are described in [Mathiot and Jourdain (2023)](https://doi.org/10.5194/egusphere-2023-1606) and were initially provided on [https://doi.org/10.5281/zenodo.8139775](https://doi.org/10.5281/zenodo.8139775). They correspond to the monthly anomaly of the 2260-2299 mean (SSP5-8.5) with respect to the 1975-2014 mean (historical) in member r1i1p1f1 of the IPSL-CM6-LR simulations [(Boucher et al., 2020)](https://doi.org/10.1029/2019MS002010).

The anomalies to add to the present-day reanalysis forcing in MISOMIP2's A1vw and W1vw experiments are provided as 3-hourly annual climatologies on the JRA55 lon-lat grid for the following variables:

**dhuss**: Near-Surface Specific Humidity anomaly.
**dpr**: Precipitation anomaly at surface; includes both liquid and solid phases from all types of clouds (both large-scale and convective).
**dprsn**: Solid precipitation anomaly at surface; includes precipitation of all forms of water in the solid phase.
**dps**: Surface Air Pressure anomaly.
**drlds**: Surface Downwelling Longwave Radiation anomaly.
**drsds**: Surface Downwelling Shortwave Radiation anomaly.
**dtas**: Near-Surface Air Temperature anomaly.
**duas**: Eastward Near-Surface Wind anomaly.
**dvas**: Northward Near-Surface Wind anomaly.
The anomalies are provided for a 365-day year. If the present-day forcing used in MISOMIP2 contains leap years, then the 28-February forcing should be repeated on February 29th.

 

### Ocean forcing perturbation (lateral boundary conditions) (A1vw, W1vw)

```
Ocean_p_*_climatology_MISOMIP2.nc
Ocean_vw_*_climatology_MISOMIP2.nc
```

These files are needed to prescribe an anomaly at the lateral boundaries of regional ocean and sea-ice models in the A1vw and W1vw experiments. The data come from the global 0.25° NEMO simulations described in [Mathiot and Jourdain (2023)](https://doi.org/10.5194/egusphere-2023-1606), including a simulation forced by the aformentioned perturbation of the atmospheric forcing. 

Given that the method to do this is open and may be done either in the physical space or in the (T,S) space, we provide both the present-day (Oceanp) and the very warm future (Oceanvw) monthly climatologies rather than the anomalies. Variables are gathered in 5 types of files:

* **seaice files**: sea ice fraction, thickness, velocities, snow thickness on ice [at **T points**].
* **bsf files**: barotropic stream function [at **F points**].
* **gridT files**: temperature, salinity, SSH [at **T points**].
* **gridU files**: x-ward ocean velocity [at **U points**].
* **gridV files**: y-ward ocean velocity [at **V points**].

The NEMO grid (eORCA025.L121) is not a regular lon-lat grid, it is stretched at high southern latitudes, uses partial steps for the deepest levels, and is on a C-grid. We believe that directly interpolating from the eORCA grid to the users grid will minimise the loss of information, so we do not provide a regridded dataset. Note that we only provide the southern hemisphere data to limit file sizes.

The grid information is provided in ```Ocean_mesh_mask_eORCA025.L121.nc```:

* glamt, glamu, glamv, glamf : longitude at T, U, V, F points (degree east).
* gphit, gphiu, gphiv, gphif : latitude at T, U, V, F points (degree north).
* e1t, e1u, e1v, e1f : mesh size along x for the 4 types of meshes (meters).
* e2t, e2u, e2v, e2f : mesh size along y for the 4 types of meshes (meters).
* e3t_0, e3u_0, e3v_0 : mesh size along z (meters).
* tmask, umask, vmask, fmask : mask values for the 4 types of meshes (=1 for ocean, =0 otherwise).

Note that the x-ward velocity (vozocrtx) and the y-ward velocity (vomecrty) are on different grids (U and V points, respectively) and need to be rotated to the target grid directions. We recommend using the barotropic stream function (BSF) to derive barotropic velocities at the lateral boundary (volume transport between two points directly given by the difference in BSF between these two points, and velocity directions so that vertically integrated velocities are defined as U=∆_y BSF and V=-∆_x BSF) and using the 3d velocities only for the baroclinic component (note that we provide the full velocities). In case this is needed, NEMO is a Boussinesq model with an ocean density of 1026 kg m-3.

 

### Perturbed ice shelves geometry (Ocean-A2f, Ocean-W2f)

```
MISOMIP2_Ocean-x2f.nc
```

The future ice draft in A2f is based on a 200-year simulation of the coupled ice-ocean model Úa-MITgcm, starting from a present-day ice-sheet geometry and forced by constant, shallow thermocline conditions on the Amundsen continental shelf [(DeRydt and Naughten 2023)](https://doi.org/10.5194/egusphere-2023-1587). For the W2f experiment, the future ice draft is based on an unpublished 300-year simulation of the coupled ice-ocean model Úa-MITgcm. The model configuration is identical to the abrupt-4xCO2 experiment described in [Naughten et al. (2021)](https://doi.org/10.1038/s41467-021-22259-0), but extended from 150 to 300 years based on a new timeseries of atmospheric and ocean boundary conditions from the UKESM-1-0-LL CMIP6 ensemble. The bathymetry for the A2f and W2f experiments is identical to the A2p and W2p experiments, i.e. BedMachine-Antarctica-v3 [(Morlighem 2022)](https://doi.org/10.5067/FPSU0V1MWUB6).

The provided dataset is formatted exactly as [BedMachine-Antarctica-v3](https://doi.org/10.5067/FPSU0V1MWUB6)  which is used for both the Ocean-A2p and Ocean-W2p experiments.

NSIDC provides matlab and python scripts to interpolate these data onto longitude-latitude grids: [https://github.com/nsidc/nsidc0756-scripts](https://github.com/nsidc/nsidc0756-scripts)
