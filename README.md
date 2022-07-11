#### Counts for the OceanSITES Dashboards

Data dashboards for the [OceanSITES Air Sea Fluxes](https://data.pmel.noaa.gov/oceansites/airseafluxes/) and 
[Long-term timeseries](https://data.pmel.noaa.gov/oceansites/lts/) operate by allowing the users to select the type
of data they wish to explore and a time range of interest. Once these are selected the dashboard will up date the
display of platform locations to show where there are data for the selected parameter and time range. 

In order to perform this operation quickly the dashboard needs access to pre-computed counts of the number
of observations for each variable in the data set. We have chosen to use monthly counts. This code will read the .json
file which defines the sites (see: the [lts](https://github.com/NOAA-PMEL/lts) and
[flux](https://github.com/NOAA_PMEL/flux) for the .json config file of sites) and makes counts for each platform
grouped by collection. The resulting data sets can be found in 
[PMEL ERDDAP](https://data.pmel.noaa.gov/pmel/erddap/search/index.html?page=1&itemsPerPage=1000&searchFor=NOBS).

#### Legal Disclaimer
*This repository is a software product and is not official communication
of the National Oceanic and Atmospheric Administration (NOAA), or the
United States Department of Commerce (DOC).  All NOAA GitHub project
code is provided on an 'as is' basis and the user assumes responsibility
for its use.  Any claims against the DOC or DOC bureaus stemming from
the use of this GitHub project will be governed by all applicable Federal
law.  Any reference to specific commercial products, processes, or services
by service mark, trademark, manufacturer, or otherwise, does not constitute
or imply their endorsement, recommendation, or favoring by the DOC.
The DOC seal and logo, or the seal and logo of a DOC bureau, shall not
be used in any manner to imply endorsement of any commercial product
or activity by the DOC or the United States Government.*