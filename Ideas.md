# Understanding-MHWs-in-case-region

According to our previous findings of 7 types of MHW vertical structures, we found that more thermocline MHWs with cold surface (negative sst anomaly) occured in the tropical Pacific Ocean than other regions. 
<img width="3875" height="2926" alt="GlobDist_MHW_byclusters_Dominant (1)" src="https://github.com/user-attachments/assets/00732c06-49db-4334-b21c-03629f23860a" />



To understand why these subsurface MHWs predominate the tropical Pacific, we are going to take a look into a small region (5S-10S, 160E-170E)。
- First, we use the daily ocean temperature (1 degree resolution) from BRAN2020 reanalysis dataset (1993.1.1-2022.12.31) to identify MHW events over depths, using Hobday et al definition. -> we found most frequent MHWs occurred at surface, while most intense MHWs occurred near the thermocline. Thermocline MHWs don't have surface expressions. 
- Second, to compare the vertical structure of surface MHWs and thermocline MHWs, we examined their severity profiles. We found surface MHWs concentrated within the mixed layer; thermocline MHW exist below the mixed layer and across great depths. Anomalously shallow MLD is found during surface MHWs. Anomalous deep MLD and TCD are both found during thermocline MHWs.  Surface severity has median value of -0.2, indicating there are cold surfaces than warm surfaces during thermocline MHWs.
- Third, we split thermocline MHWs into three types: MHWs with cold surface (negative sst anomaly), with warm surface (positive sst anomaly), and with mixed surface.

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
