---
layout: page
title: MIPkit-A (Amundsen)
date: 02-11-2023
---

Observational data kit gathered and reprocess to facilitate the evaluation of ocean models as part of [MISOMIP2](https://climate-cryosphere.org/about-15/).

**This entire dataset should be cited as** the MISOMIP2 MIPkit-A dataset [http://doi.org/10.5281/zenodo.10062356](http://doi.org/10.5281/zenodo.10062356) that includes data collected through multiple cruises of the Nathaniel B. Palmer (United States Antarctic Program), James C. Ross (British Antarctic Survey and Natural Environment Research Council), Araon (Korea Polar Research Institute), Oden (Swedish Polar Research) and Polarstern (Alfred Wegener Institute, Germany).

For more specific use of some of the MIPkit-A data, we encourage people to cite the original data referenced below.

### Oce3d\_MIPkitA\_* : 3-dimensional temperature and salinity (horizontal slices every 100m)

The hydrographic properties provided on horizontal sections at 15 depths come from the CTD measurements obtained during cruises of the following icebreaker research vessels: Nathaniel B. Palmer (United States Antarctic Program), James C. Ross (British Antarctic Survey and Natural Environment Research Council), Araon (Korea Polar Research Institute), Oden (Swedish Polar Research) and Polarstern (Alfred Wegener Institute, Germany). In this MIPkit, we have gathered data for the first months of 2009 ([Jacobs 2009](http://doi.org/10.7284/905547)), 2010 ([Swedish Polar Research Secretariat 2010](http://snd.gu.se/en/catalogue/dataset/ecds0220-1); [Gohl 2015](https://doi.org/10.1594/PANGAEA.847944)), 2012 ([Kim et al. 2012](https://repository.kopri.re.kr/handle/201206/4603)), 2014 ([Heywood 2014](https://www.bodc.ac.uk/resources/inventories/cruise_inventory/report/13405/); [Ha et al. 2014](https://repository.kopri.re.kr/handle/201206/4605)), 2016 ([Kim et al. 2016](https://ftp.nmdc.no/nmdc/UIB/Mooring/20181213/ANA06B_cruise_report.pdf)), 2017 ([Gohl 2017](http://doi.org/10.2312/BzPM_0712_2017)), 2018 ([Kim et al. 2018](https://repository.kopri.re.kr/handle/201206/9441)), 2019 ([Larter et al. 2019](http://doi.org/10.7284/908147)) and 2020 ([Wellner, 2020](http://doi.org/10.7284/908803)).

### OceSec\<n\>\_MIPkitA\_* : vertical sections

The first vertical (**OceSec1**) section where we provide hydrographic data in the Amundsen Sea starts across the continental shelf break and follows the Eastern Pine Island Trough southward until Pine Island Ice Shelf. This section was monitored by the following cruises: N.B. Palmer in January 2009, Polarstern in March 2010 and Araon in February-March 2012 ([Jacobs et al. 2011](https://doi.org/10.1038/ngeo1188); [Gohl 2015](https://doi.org/10.1594/PANGAEA.847944); [Dutrieux et al. 2014](https://doi.org/10.1126/science.1244341)). The second vertical section (**OceSec2**) starts across the continental shelf break and follows the Dotson-Getz Trough southward until the Dotson Ice Shelf. It was monitored by the aforementioned Araon expeditions in 2010–2011 and early 2012 ([Kim et al. 2017](http://dx.doi.org/10.1016/j.csr.2016.09.005)).

The files OceSec\<n\>\_model\_lon\_lat.csv contain the coordinates (longitude, latitude) at which model data should be interpolated to be compared to the observational sections.

### OceMoor\<n\>\_MIPkitA\_* : moorings

The first mooring site (**OceMoor1**) is located near the northern part of the Pine Island ice shelf front (102.07°W, 74.87°S) and captures the thermocline variability from 2012 to 2018 ("iSTAR-8" in NERC iSTAR program, and "pig-n" in NERC Ocean Forcing Ice Change Program). The second mooring site (**OceMoor2**)is located near the southern part of the Pine Island ice shelf front (102.15°W, 75.05°S), was monitored between 2009 and 2016, then in 2019–2020 through the following moorings: "BSR-5" (Buoy Supported Riser; [Jacobs 2009](http://doi.org/10.7284/905547)), "iSTAR-9" ([NERC iSTAR Program](https://www.istar.ac.uk)), and "pig-s" (NERC Ocean Forcing Ice Change Program). This second site experienced a strong deepening of the thermocline in 2012–2013 ([Webber et al. 2017](https://doi.org/10.1038/ncomms14507)), then a more moderate deepening in 2016. These two mooring sites are located only 20 km from each other, show distinct mean thermocline depth and more consistent variability ([Joughin et al. 2021](https://doi.org/10.1126/sciadv.abi5738)).

The third mooring observation (**OceMoor3**, "trough-e" in NERC Ocean Forcing Ice Change Program) used in MISOMIP is at the eastern Pine Island trough (102.55°W, 71.33°S). The eastern trough is considered to be the entrance of mCDW reaching the Pine Island Ice Shelf ([Jacobs et al. 2011](https://doi.org/10.1038/ngeo1188); [Nakayama et al. 2013](https://doi.org/10.1016/j.dsr.2013.04.001); [Webber et al. 2017](https://doi.org/10.1038/ncomms14507)) but only two years of mooring observation was conducted from 2014-2015 due to important sea ice cover. The fourth mooring site (**OceMoor4**) used in MISOMIP is at the western Pine Island trough (113.05°W, 71.56°S). Several mooring observations were conducted within 2 km of each other, allowing us to observe thermocline variability from 2009 to 2016 with one year gap in 2011: "BSR-12" ([Jacobs 2009](http://doi.org/10.7284/905547)), "iSTAR-1" ([NERC iSTAR Program](https://www.istar.ac.uk)), and "trough-w" (NERC Ocean Forcing Ice Change Program).

### To know more on how these files were prepared:

The archive **example\_routines.zip** contains example of Matlab routine that were used to prepare the MIPkit-A data.

### References

* Dutrieux, P., De Rydt, J., Jenkins, A., Holland, P. R., Ha, H. K., Lee, S. H., Steig, E. J., Ding, Q., Abrahamsen, E. P., and Schröder, M.: Strong sensitivity of Pine Island ice-shelf melting to climatic variability, Science, 343, 174–178, 2014.

* Gohl, K.: Station list and links to master tracks in different resolutions of POLARSTERN cruise ANT-XXVI/3, Wellington - Punta Arenas, 2010-01-30 - 2010-04-05, Tech. rep., Alfred Wegener Institute, Helmholtz Centre for Polar and Marine Research, Bremerhaven, [https://doi.org/10.1594/PANGAEA.847944](https://doi.org/10.1594/PANGAEA.847944), 2015.

* Gohl, K.: The Expedition PS104 of the Research Vessel POLARSTERN to the Amundsen Sea in 2017, Reports on polar and marine research, Tech. rep., Alfred Wegener Institute for Polar and Marine Research, Bremerhaven, [http://doi.org/10.2312/BzPM_0712_2017](http://doi.org/10.2312/BzPM_0712_2017), 2017.

* Ha, H. K., Kim, T. W., Lee, H. J., Kang, C. Y., Hong, C. S., Wåhlin, A. K., Rolandsson, J., Karen, O., and Miles, T.: The Amundsen Sea Expedition (ANA04B): IBRV Araon, 24 December 2013 – 25 January 2014 – Chapther 1: Physical Oceanography, Tech. rep., Korea Polar Research Institute, Incheon, [https://repository.kopri.re.kr/handle/201206/4605](https://repository.kopri.re.kr/handle/201206/4605), 2014.

* Heywood, K. 690 J.: JR294/295 Cruise Report, Ice Sheet Stability Programme (iSTAR), RRS James Clark Ross, 26th February – 8th March 2014, Amundsen Sea, Tech. rep., Natural Environment Research Council (NERC), [https://www.bodc.ac.uk/resources/inventories/cruise_inventory/report/13405/](https://www.bodc.ac.uk/resources/inventories/cruise_inventory/report/13405/), 2014.

* Jacobs, S.: Cruise NBP0901, RVIB Nathaniel B. Palmer, Jan 05 – Feb 26 2009, Tech. rep., United States Antarctic Program, [http://doi.org/10.7284/905547](http://doi.org/10.7284/905547), 2009.

* Jacobs, S. S., Jenkins, A., Giulivi, C. F., and Dutrieux, P.: Stronger ocean circulation and increased melting under Pine Island Glacier ice shelf, Nature Geoscience, 4, 519–523, 2011.

* Joughin, I., Shapero, D., Smith, B., Dutrieux, P., and Barham, M.: Ice-shelf retreat drives recent Pine Island Glacier speedup, Science Advances, 7, eabg3080, 2021.

* Kim, T. W., H, H. K., and Hong, C. S.: The Amundsen Sea Expedition (ANA02C): IBRV Araon, 31 January 2012 – 20 March 2012 – Chapther 1: Hydrographic Survey, Tech. rep., Korea Polar Research Institute, Incheon, [https://repository.kopri.re.kr/handle/201206/4603](https://repository.kopri.re.kr/handle/201206/4603), 2012.

* Kim, T. W., Cho, K. H., Kim, C. S., Yang, H. W., La, H. S., Lee, J. H., Kim, D. K., Jung, J. H., Wåhlin, A. K., Assmann, K. M., Darelius, E., Abrahamsen, E. P., and Waite, N.: The Amundsen Sea Expedition (ANA06B): IBRV Araon, 6 January – 23 February 2016 – Chapther 1: Physical Oceanography in Amundsen Sea, Tech. rep., Korea Polar Research Institute, Incheon, [https://ftp.nmdc.no/nmdc/UIB/Mooring/20181213/ANA06B_cruise_report.pdf](https://ftp.nmdc.no/nmdc/UIB/Mooring/20181213/ANA06B_cruise_report.pdf), 2016.

* Kim, T.-W., Ha, H. K., Wåhlin, A. K., Lee, S., Kim, C.-S., Lee, J. H., and Cho, Y.-K.: Is Ekman pumping responsible for the seasonal variation of warm circumpolar deep water in the Amundsen Sea?, Continental Shelf Research, 132, 38–48, 2017.

* Kim, T. W., Cho, K. H., Park, T. W., Yang, H. W., Kim, Y., Assmann, K. M., Rolandsson, J., Dutrieux, P., Gobat, J., Beem, L., Richter, T., Buhl, D., and Durand, I.: The Amundsen Sea Expedition (ANA08B): IBRV Araon, 21 December 2017 – 13 February 2018 – Chapther 1: Physical Oceanography, Tech. rep., Korea Polar Research Institute, Incheon, [https://repository.kopri.re.kr/handle/201206/9441](https://repository.kopri.re.kr/handle/201206/9441), 2018.

* Larter, R., Barham, M., Boehme, L., Braddock, S., Graham, A., Hogan, K., Mazur, A., Minzoni, R., Queste, B., Sheehan, P., Spoth, M., Wåhlin, A., Bortolotto-d’Oliveira, G., Clark, R. W., Fitzgerald, V., Karam, S., Kirkham, J., Stedt, F., Zheng, Y., Beeler, C., Goodell, J., Rush, E., Snow, T., Welzenbach, L., Andersson, J., and Rolandsson, J.: Cruise NBP1902, RVIB Nathaniel B. Palmer, Jan 29 – Mar 25 2019, Tech. rep., United States Antarctic Program, [http://doi.org/10.7284/908147](http://doi.org/10.7284/908147), 2019.

* Nakayama, Y., Schröder, M., and Hellmer, H. H.: From circumpolar deep water to the glacial meltwater plume on the eastern Amundsen Shelf, Deep Sea Res. I, 77, 50–62, 2013.

* Swedish Polar Research Secretariat: Oden Southern Ocean 2009/10 - Conductivity-Temperature-Depth (CTD) Data Collected Onboard Icebreaker Oden during February through March 2010, Tech. rep., Swedish Polar Research, [http://snd.gu.se/en/catalogue/dataset/ecds0220-1](http://snd.gu.se/en/catalogue/dataset/ecds0220-1), 2010.

* Webber, B. G. M., Heywood, K. J., Stevens, D. P., Dutrieux, P., Abrahamsen, E. P., Jenkins, A., Jacobs, S. S., Ha, H. K., Lee, S. H., and Kim, T. W.: Mechanisms driving variability in the ocean forcing of Pine Island Glacier, Nature Communications, 8, 1–8, 2017.

* Wellner, J.: Cruise NBP2002, RVIB Nathaniel B. Palmer, Jan 25 2020 – Mar 08 2020, Tech. rep., United States Antarctic Program, [http://doi.org/10.7284/908803](http://doi.org/10.7284/908803), 2019.
