# Understanding-MHWs-in-tropical-Pacific

## Background
Our previous work indicates there are 7 common vertical types of large-scale MHWs in the global ocean and the tropical Pacific ocean appears to be hotspots for thermocline type with cold surface (negative sst anomaly). 
<img width="3875" height="2926" alt="GlobDist_MHW_byclusters_Dominant (1)" src="https://github.com/user-attachments/assets/00732c06-49db-4334-b21c-03629f23860a" />
## Hypothesis
Our hypothesis is these thermocline MHWs in the tropical ocean are dominated by a thermocline deepening linked to local wind-driven downwelling, planetary waves, as well as ocean warm-core eddies. And their cold surface is linked to co-occurrence of enhanced surface heat loss driven by increased wind.
## Planned Analysis 
Driven by the hypothesis, we conduct the following analysis to test whether it is right or not.

1) We first identify all extreme warm temperature profiles over tropical ocean using daily ocean temperature (1 degree resolution) from BRAN2020 reanalysis dataset (1993.1.1-2022.12.31) and then make cluster for their severity index profiles.
   - 1/ We calculate severity index (S) over all grid cells and at all depth levels in tropical ocean.
   - 2/ We pick up the profiles when S>1 at any depth and last over 5 days. Analogy to Hobday et al 2016 MHW definition. We can also test S>2 to look more extreme MHWs or S > 1 but last over 10 or 20 days to look longer MHWs. See how the threshold affects the results.
   * S > 2 means daily temperature is far over 90th climatological temperature on that given day by over 90th percentile difference to climatological mean. S > 2 here is analogous to the temperature threshold for MHW category II strong (Hobday et al. 2018).
   - 3/ Then rescaled severity profile along depths and do clustering.

2) Once we get clusters, check if there is thermocline type with cold surface or warm surface. Then exmine their spatial distributions. -> see if they are similar to our previous findings for large-scale MHWs. If different, why? 
  
3) For each types profiles,  split to onset and decay phrases.
   * correlation between aomalous local Ekman pumping, and anomalous local temperature tendency over depths or anomalous thermocline depth changes -> check wind effect on thermocline
   * correlation between anomalous surface heat flux components and sea surface temperature anomaly -> check heat flux effect on surface
   * correlation between sea surface height anomaly and thermocline depth anomaly. Examine the spatial-temporal patterns of sea surface height to see if it is related to planetary waves? Can the sea surface height anomaly related to eddies? Need to check eddy track from AVISO dataset (https://www.aviso.altimetry.fr/en/data/products/value-added-products/global-mesoscale-eddy-trajectory-product.html).

## Data
### BRAN2020 DATA 
- Data acess on NCI: /g/data/gb6/BRAN/BRAN2020/daily. 
- Data horizontal resolution: 0.1 degree. -> Need regriding onto 1*1 grid point.
- Website: https://geonetwork.nci.org.au/geonetwork/srv/eng/catalog.search#/metadata/f9372_7752_2015_3718
- Literatures of BRAN2020: https://essd.copernicus.org/articles/13/5663/2021/#bib1.bibx8
#### Daily averaged ocean fields (temperature, sea level, mixed layer depth)
- ocean temperature.
- sea level ~ Files: ocean_eta_t_1993_01.nc 
- mixed layer depth ~ Files: ocean_mld_2017_08.nc
- Note: MLD is the depth over which the buoyancy exceeds a threshold of 0.0003 m/s2, as described by Griffies (2012). It is roughly equivalent to a density threshold of Δρ ≈ 0.03 kg/m³.
  
#### Daily averaged atmospheric flux fields 
- Data files: ocean_force_2022_02.nc
##### Heat Fluxe Parameters:
- longwave flux into ocean (<0 cools ocean) ~ lw_heat
- sensible heat into ocean (<0 cools ocean) ~ sens_heat
- latent heat flux into ocean (<0 cools ocean) ~ evap_heat
- shortwave flux into ocean (>0 heats ocean) ~ swflx
##### Freshwater Flux Parameters:
- precip-evap via sbc (liquid, frozen, evaporation) ~pme_sbc
- mass flux from evaporation/condensation (>0 enters ocean) ~evap
- liquid precip (including ice melt/form) into ocean (>0 enters ocean) ~ lprec
##### Momentum Flux Parameters:
- i-directed wind stress forcing u-velocity ~ tau_x
- j-directed wind stress forcing v-velocity ~ tau_y

- It is noted that BRAN2020 ocean model OFAM3 is forced by JRA55 atmospheric conditions and compute the atmospheroc fluxes via bulk formula.

## Initial results
#### Overview of subsurface temperature extremes and MHWs
<img width="3050" height="2286" alt="MHW_severity_hovmoller_MHWintensity_at_13depths" src="https://github.com/user-attachments/assets/23075cc8-584d-4638-ba9d-52471df362e9" />

#### Statistics of MHWs at individual depths
<img width="3570" height="866" alt="MHW_features_at_13depths" src="https://github.com/user-attachments/assets/33557dc1-c09b-4c36-bcc7-369c66d6e60a" />

#### Below is severity distribution over depths when surface water in MHW conditions (a) and 200m water in MHW conditions (b)
<img width="2970" height="1166" alt="surfaceMHW_vs_200mMHW_severity_profiles" src="https://github.com/user-attachments/assets/6ba97f24-eaf9-4378-9664-327482a406b7" />

#### I split the severity profiles for 200m-MHWs into two types based on their sea surface temperature:  warm-surface and cold-surface 
<img width="2585" height="1407" alt="200mMHW_severity_profiles_warm_vs_cold" src="https://github.com/user-attachments/assets/607b88e8-5688-4701-acdd-102295813ddf" />

#### See how the cold-surface profiles distribute over time and MHW events
<img width="3608" height="2367" alt="200mMHWs_sst_anom_timeevolution (1)" src="https://github.com/user-attachments/assets/182f4459-2fa7-429a-9157-aae6bff1930f" />



- ERA5 daily mean surface heat flux (latent heat flux, sensible heat flux, net shortwave radiation, net longwave radiation, and their sum) from 1993Jan to 2022Dec. -> Daily anomalies referecened to climatology of 1993-2022
- Copernicus marine Climate Change Service (C3S) sea level anomaly gridded data from 2003.1.1 to 2006.12.31  The sea level anomaly is provded with respect to the mean sea level during 1993-2012.
- ERA5 daily 10-m wind speed during 1993-2020. Calculate wind stress and ekman pumping anomaly during 2003-2006.
