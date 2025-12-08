# Chapter 4: Understanding-MHWs-in-tropical-Pacific

## Background
Our previous work indicates there are 7 common vertical types of large-scale MHWs in the global ocean and the tropical Pacific ocean appears to be hotspots for thermocline type with cold surface (negative sst anomaly). 
<img width="3875" height="2926" alt="GlobDist_MHW_byclusters_Dominant (1)" src="https://github.com/user-attachments/assets/00732c06-49db-4334-b21c-03629f23860a" />
<img width="5308" height="3649" alt="7clustering_severity_profile_mean_std (5)" src="https://github.com/user-attachments/assets/1d71d4ac-7843-46f1-8520-4c06655145b2" />

Correlation analysis with Nino3.4 index suggests more TCL-cold MHW types tend to occur during Lanina years (correlation coefficient = -0.23, p value < 0.01) and mostly found in the western tropical Pacific and eastern Indian Ocean, as well as south Indian Ocean.
<img width="4706" height="3409" alt="7MHWprofileTypes_Nino34_correlation_maps" src="https://github.com/user-attachments/assets/320da746-f26c-48b9-9df3-f6905baad78e" />

During 2010 November when Lanina persisted, one significant TCL-cold type MHW (#278) occurred over the western tropoical Pacific and eastern tropical Indian Ocean. 
In its central regions (90E-150E), where surface water is anomalously warm, MHWs are dominated by mixed-layer, deep and submerged-verywarm types.
While on the west (40-90E) and east sides (150-180E), where surface is cold anomaly, MHWs are dominated by TCL-cold types, although SM-cold type is also present in the equatorial Inidna Ocean. 
<img width="3510" height="1524" alt="2010Nov_No287_MHWcluster_distribution" src="https://github.com/user-attachments/assets/dc51b881-e3cc-43c0-9026-26210bd97774" />

### La Nina composite plots
47 La Nina months are identified when Nino3.4 index exceeds its standard deviation during 1993-2020.
<img width="826" height="385" alt="image" src="https://github.com/user-attachments/assets/ed6f11a7-8360-4df9-8407-1ff82a477942" />
After a removal the linear temporal trend of the temperature, we calculated monthly temperature anomaly at each depth level and calculated monthly thermocline depth anomaly.
Then we took the average of thermocline depth anomaly and 5m temperature anomaly among all La Nina months. The countours show the counts of TCL-cold MHW profile within each 5 lat * 10 lon grid cell.   

<img width="1725" height="465" alt="image" src="https://github.com/user-attachments/assets/c24343b5-039e-4a61-9488-8262543b17f1" />



The 2010 November MHW example suggtes that it's not true that all western tropical ocean during lanina are warm at surface. Some can be cold at surface, but subsurface gets warm. Why?  Many potential mehcanisms: 1) increased cloud cover reduces the incoming solar radiation, so cools the surface. 2) increased wind speed enhances the evaporative heat loss and cools the surface. 3) increased wind stress curl enhances the upwelling and cools the surface. but unlikely since thermocline warming usually suggets a deepening. 2) Increased transport of surface warm water from east to west deepens the thermocline on west, makes subsurface warming.  
To examine whether these process likely drive TCL-cold MHWs in Lanina, we can make a regression between nino3.4 index and interested atmospheric and oceanic variables, to see how these processes change. Explore if they can explain the TCL-cold hotspots. Variables include cloud cover, wind speed, wind stress curl, thermocline depth, net shortwave radiation.


### Regression map between Nino3.4 index (X) and thermocline depth (Y).
During Elnino, thermocline gets deepening on eastern tropical Pacific and southwest tropical Pacific, while gets shallow over west tropical Pacific with an eastward extension in 10-25S latitude bands. During Lanina, the pattern is opposite with deepening of thermocline over western tropical Pacific and extension area and shoaling over eastern and southwest tropical Pacific. 
<img width="3906" height="1708" alt="regslope_nino34_tcd_tropicalPacific" src="https://github.com/user-attachments/assets/22a1d346-26a7-445c-af09-20ab42e4a6dd" />

### Regression map between Nino3.4 index (X) and sst (Y).
During Elnino, surface warming is found over central and eastern tropocal Pacific, while cooling is found in western tropcial ocean with an eastward extension in 10-25S latitude bands. During lanina, the pattern is opposite with surface cooling over central and eastern tropocal Pacific, and warming in western tropcial ocean with an eastward extension in 10-25S latitude bands. 
<img width="3880" height="1707" alt="regslope_nino34_sst_tropicalPacific (1)" src="https://github.com/user-attachments/assets/f5808c66-f345-42c6-8985-b1515fc3dfef" />

### Regression map between Nino3.4 index (X) and net shortwave radiation flux (Y).
There's a west-east dipole pattern over equatorail pacific ocean. During Elnino, incoming solar radiation is decreased (blue) across the braod east regions (150E-100W) cooling the ocean and increased (red) in the west regions (90E-150E) warming the ocean. During Lanina, pattern is opposite with warming across the east regions and cooling in the west regions.
<img width="3949" height="1707" alt="regslope_nino34_swflx (1)" src="https://github.com/user-attachments/assets/c73ca671-7a2e-48cf-b8c7-f026bb2dec79" />


### Regression map between Nino3.4 index (X) and cloud cover (Y).
There is a west-east dipole over equatorial pacific consistent with net shorwave radiation flux. During Elnino, it's more cloudy across the braod east regions (150E-100W), which reduces the incoming solar radiation, cooling the ocean. While it's more clear sky in the west regions (90E-150E), that allows more solar radiation reach the ocean, warming the ocean. Lanina has opposite pattern with cloudy sky  in the west regions (90E-150E) and clear sky across the braod east regions (150E-100W).
<img width="3937" height="1709" alt="regslope_nino34_cloudcover" src="https://github.com/user-attachments/assets/cd92388e-bc07-48b2-9a81-f6d7c2d11c2b" />


### Regression map between Nino3.4 index (X) and net latent heat flux (Y). 
During Elnino, evaporation is increased (blue) over the east equatorial Pacific (150W-80W) amd southwest trpical pacific, cooling the ocean. While evaporation is decreased (red) over the west equatorail Pacific (160E-150W) warming the ocean. During lanina, pattern is opposite with warming over the east equatorial Pacific (150W-80W) amd southwest trpical pacific and cooling over the west equatorail Pacific (160E-150W).
<img width="3952" height="1707" alt="regslope_nino34_lhflx" src="https://github.com/user-attachments/assets/46a3b3fc-1afc-4239-b23f-b963e432971e" />

### Regression map between Nino3.4 index (X) and 10-m Wind speed (Y).
During Elnino, wind gets weaker in the central equatorial Pacificm, desceasing the ocean latent heat loss and warming the ocean. While wind gets stronger over the east and west equatorial pacific and  southwest tropical Pacific, enhancing the ocean latent heat loss, cooling the ocean. During Lanina, pattern is opposite with stronger wind and increased ocean latent heat loss in the central Pacific, and weaker wind and reduced ocean latent heat loss over the east and west equatorial Pacific and southwest tropical Pacific.
<img width="3893" height="1708" alt="regslope_nino34_U10m" src="https://github.com/user-attachments/assets/810ca295-d3ea-400f-8edb-692d5d90dfbb" />

### Regression map between Nino3.4 index (X) and Wind-induced Ekman pumping velocity (Y).
During Elnino, when upwelling 
<img width="3941" height="1709" alt="regslope_nino34_Ekman_upwelling" src="https://github.com/user-attachments/assets/928e9286-8990-4d40-bf2e-df5f18296cff" />


## Hypothesis
Our hypothesis is these thermocline MHWs in the tropical ocean are dominated by thermocline deepening, driven by multiple mechanisms, like local wind-driven downwelling, planetary waves, as well as ocean warm-core eddies. These MHWs have a preference of cold surface, which could be linked to co-occurrence of enhanced evaporative surface heat loss driven by increased wind.
## Planned Analysis 
Driven by the hypothesis, we conduct the following analysis to test whether it is right or not.

1) We first identify all extreme severity profiles over tropical ocean using daily ocean temperature (1 degree resolution) from BRAN2020 reanalysis dataset (1993.1.1-2022.12.31) and then do clustering.
   - 1/ I calculate severity index (S) over all grid cells and at all depth levels in tropical Pacific.
   - 2/ I pick up the profiles when S>2 at any depth and last over 15 days (first quick test).
   * S > 2 means daily temperature is far over 90th climatological temperature on that given day by over 90th percentile difference to climatological mean. S > 2 here is analogous to the temperature threshold for MHW category II strong (Hobday et al. 2018).
   * Small severity threshold and short duration gives more MHW profiles on each grid cell. See how the threshold affects the results.
   - 3/ Then rescaled severity profile along depths and do clustering.

2) Once we get clusters, check if there is thermocline type with cold surface or warm surface. Then exmine their spatial distributions. -> see if they are similar to our previous monthly MHW results. If different, why? 
  
3) Spot out the thermocline-cold type MHWs, split to onset and decay phrases.
   * check Ekman pumping effect on subsurface temperature & thermocline depth: correlation between aomalous local Ekman pumping, and anomalous local temperature tendency over depths or anomalous thermocline depth changes
   * check heat flux effect on surface temperaure: correlation between anomalous surface heat flux components and sea surface temperature anomaly 
   * check planetary waves/eddies effect on subsurface temperature & thermocline depth: correlation between sea surface height anomaly and thermocline depth anomaly.
   * Examine the spatial-temporal patterns of sea surface height to see if it is related to planetary waves? Can the sea surface height anomaly related to eddies? Check eddy track from AVISO dataset? (https://www.aviso.altimetry.fr/en/data/products/value-added-products/global-mesoscale-eddy-trajectory-product.html).

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
- longwave flux into ocean (<0 cools ocean, unit: "W/m^2") ~ lw_heat
- sensible heat into ocean (<0 cools ocean, unit: "W/m^2") ~ sens_heat
- latent heat flux into ocean (<0 cools ocean, unit: "W/m^2") ~ evap_heat
- shortwave flux into ocean (>0 heats ocean, unit: "W/m^2") ~ swflx
##### Freshwater Flux Parameters:
- precip-evap via sbc (liquid, frozen, evaporation, unit: (kg/m^3)*(m/sec)) ~pme_sbc
- mass flux from evaporation/condensation (>0 enters ocean, unit:(kg/m^3)*(m/sec)) ~evap
- liquid precip (including ice melt/form) into ocean (>0 enters ocean, unit: (kg/m^3)*(m/sec)) ~ lprec
##### Momentum Flux Parameters:
- i-directed wind stress forcing u-velocity (unit: "N/m^2")~ tau_x
- j-directed wind stress forcing v-velocity (unit: "N/m^2")~ tau_y
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
