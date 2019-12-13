# ANTBGM
Transation towards Bedmap3(or BedMarchine:Antarctica), ANTGG2?, ADMAP3

The purpose of this dataset is filling data gap in current continental scale compliation using pubulic avaiable individual survey.


# Bedmap21

Since the publication of Bedmap2(2013), Ice Penetrating Radar data has revealed the detail bedrock elevation information in the South Pole, Centre Marine Byrd Land, Recovery Lakes Glacier, Dornning Maud Land. These bed informations are estimated by satelite Free-Air gravity/topography transation in Bedmap2. Here, follow the workflow of building Bedmap2, new IPR data is merged with the exsit bed information.

Whether RTopo-2.0.4 data is better to reconstruct topography (with better bathymetry data) 
Schaffer, Janin; Timmermann, Ralph; Arndt, Jan Erik; Rosier, Sebastian H R; Anker, Paul G D; Callard, S Louise; Davis, Peter E D; Dorschel, Boris; Grob, Henrik; Hattermann, Tore; Hofstede, Coen M; Kanzow, Torsten; Kappelsberger, Maria; Lloyd, Jerry M; Ó'Cofaigh, Colm; Roberts, David H (2019): An update to Greenland and Antarctic ice sheet topography, cavity geometry, and global bathymetry (RTopo-2.0.4). PANGAEA, https://doi.org/10.1594/PANGAEA.905295, Supplement to: Schaffer, Janin; Kanzow, Torsten; von Appen, Wilken-Jon; von Albedyll, Luisa; Arndt, Jan Erik; Roberts, David H (in review): Bathymetry constrains ocean heat supply to Greenland's largest glacier tongue. Nature Geoscience

Work Flow:

1. Gather new radar information, make a mask with 50 Km away from new radar 
2. Mask original ice thickness data with 20 Km away from Radar Measurement in Bedmap2.
3. Regridding Ice thickness grid from Bedmap2 with new ice thickness data by Topo to Raster (ANUDEM algorithm: thin plate spline) in Arcpy.

With the publication of Bedmarchine Antarctica. The bed information is current the best avaliable dataset. The only datagap is in East Princess Elizabeth Land.


# AntGG11

A interesting paper talk about the gravity data compilation in Antarctica.

Zingerle, P., Pail, R., Scheinert, M., et al. (2019). Evaluation of terrestrial and airborne gravity data over Antarctica – a generic approach. Journal of Geodetic Science, 9(1), pp. 29-40. Retrieved 4 Dec. 2019, from doi:10.1515/jogs-2019-0004






# ADMAP21
