# Understanding-MHWs-in-case-region

Our previous work indicates there are 7 common vertical types of large-scale MHWs in the global ocean and the tropical oceans appear to be hotspots for thermocline type with cold surface (negative sst anomaly). 
<img width="3875" height="2926" alt="GlobDist_MHW_byclusters_Dominant (1)" src="https://github.com/user-attachments/assets/00732c06-49db-4334-b21c-03629f23860a" />

Our hypothesis is these thermocline MHWs in the tropical ocean are dominated by a thermocline deepening linked to local wind-driven downwelling, planetary waves, as well as ocean warm-core eddies. And their cold surface is linked to co-occurrence of enhanced surface heat loss driven by increased wind.

Driven by the hypothesis, we conduct the following analysis to test whether it is right or not.

1) We first identify all extreme warm temperature profiles over tropical ocean using daily ocean temperature (1 degree resolution) from BRAN2020 reanalysis dataset (1993.1.1-2022.12.31) and then make cluster for their severity index profiles.
1. We calculate severity index (S) over all grid cells and at all depth levels in tropical ocean.
2. We pick up the profiles when S>1 at any depth and last over 5 days. Analogy to Hobday definition. We can also test S>2 to look more extreme MHWs or S > 1 last over 10 or 20 days to look longer MHWs. See how the threshold affects the results.
   * S > 2 means daily temperature is far over 90th climatological temperature on that given day by over 90th percentile difference to climatological mean. S > 2 here is analogous to the temperature threshold for MHW category II strong (Hobday et al. 2018).
3. Then we did cluster over all these MHW-related extreme temperatore profiles.

2) Once we get clusters, check if there is thermocline type with cold surface or warm surface. Then exmine their spatial distributions. -> see if they are similar to our previous findings for large-scale MHWs. If different, why? 
  
3) For thermocline-cold types profiles, do correlation local Ekman pumping, to local temperature tendency and thermocline depth changes -> check wind effect
4) Do correlation of sea surface height to thermocline depths 
5) 

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


To explore the oceanic and atmospheric drivers of two events, I downloaded the data below. All these dataset have 1/4 spatial resolution. daily ERA5 air-sea heat fluxes and wind speed, daily C3S sea level anomaly.
- ERA5 daily mean surface heat flux (latent heat flux, sensible heat flux, net shortwave radiation, net longwave radiation, and their sum) from 1993Jan to 2022Dec. -> Daily anomalies referecened to climatology of 1993-2022
- Copernicus marine Climate Change Service (C3S) sea level anomaly gridded data from 2003.1.1 to 2006.12.31  The sea level anomaly is provded with respect to the mean sea level during 1993-2012.
- ERA5 daily 10-m wind speed during 1993-2020. Calculate wind stress and ekman pumping anomaly during 2003-2006.
