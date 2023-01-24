# OpenDSSPVPenetrationLVgrid

Simulation based on the case in: https://doi.org/10.1109/ENERGYCON.2014.6850533

The grid under study:

![image](https://user-images.githubusercontent.com/33414239/214399543-e03ef884-9448-44a4-a80d-3aeb9862c5fa.png)

The load model consists of residential loads in almost all bu ses and commercial buildings in bus 5 and 6. The load profil e s is selected for a spec if ic day during the winter with higher demand and as pecific summer day  ith high solar irradiance and ower demand. All the loads are assumed to operate at power factor of 0.9 lagging.

The PV systems are sized so that the residential load will be classified as a zero emission house (ZEH). A zero emission house has a higher or equal amount ofclean energy produced to the amount of consumed energy. Hence, ZEH can be achieved by installing PV with size based on the annual energy consumption of each load. The irradiance and temperature is a historical data from the year of 2011, obtained from API toolkit https://solcast.com/. 

![image](https://user-images.githubusercontent.com/33414239/214401290-3a9185e7-7dc0-4065-9fa6-c13544b53712.png)

Three simulation cases are performed. All the residential load is assumed to be equipped with PV system so that it becomes a ZEH The solar irradiation has the same characteristics in all cases except for winter.
  1) Winter with OLTC
      This case has the highest load of the year and negligible amount of PV production.
  2) Summer with OLTC
      This case considers low summer load and high PV production, which creates a high production consumption discrepancy, leading to higher reverse power and voltage         rise.
  3) Summer with OLTC and Increased PV at the commercial loads
      Same as in scenario 3, but with PV installed in commercial loads with capacity corresponds to the peak load of each node. A load factor of 0.5 is assumed.
      
 To run: Copy the scprit to OpenDSS and execute.
