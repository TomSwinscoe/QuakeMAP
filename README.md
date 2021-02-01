# QuakeMAP
The following python script is used to process and visualize seismic event and seismic station data in the Kiskatinaw Seismic Monitoring and Mitigation Area (KSMMA), north-east British Columbia, Canada from 2014-2018.

It is also intended to highlight the functionality of Pandas, GeoPandas and Bokeh for processing and visualizing open source georeferenced data using open source software, in particular for producing an interactive time-series map for explaratory analysis.

This python script will be updated with seismic event data from 2019-2020 once it is publicly available.

<figure>
  <p>
    <img
         src="https://github.com/TomSwinscoe/QuakeMAP/blob/main/QuakeMAP.png"
         text-align="center"
         width="465px"
         height="504px">
    </img>
  </p>
</figure>

https://tomswinscoe.github.io/index/QuakeMAP.html

#### **Data**
##### KSMMA boundary data from the British Columbia Oil and Gas Commission (BCOGC) (open source)
- ftp://ftp.bcogc.ca/outgoing/Induced%20Seismicity%20in%20KSMMA_Report%20Appendices/Appendix%20D%20-%20Mapping%20and%20Pressure%20Data%20Files/Shapefiles/General/

##### Seismic event data from the Geological Survey of Canada (GSC) (open source)
- https://geoscan.nrcan.gc.ca/starweb/geoscan/servlet.starweb?path=geoscan/fulle.web&search1=R=306292 (2014-2016)
- https://geoscan.nrcan.gc.ca/starweb/geoscan/servlet.starweb?path=geoscan/fulle.web&search1=R=326015 (2017-2018)

##### Seismic station data from the Incoporated Research Institutions for Seismology (IRIS) (open source)
- https://ds.iris.edu/gmap/#network=*&starttime=2014-01-01&maxlat=56.4811&maxlon=-119.9268&minlat=55.6528&minlon=-121.2608&drawingmode=box&planet=earth (note to only select stations where seismic data is available (A), or partially available (P), and not restricted (R), view 'more information' on the station icon. This also highlights which stations are co-located (broadband and accelerometer rather than just broadband) by the presence of a Titan instrument. For this data, this includes stations: BCH1B, BCH2B, MONT1, MONT2, MONT3, MONT6, MONT8, MONT9, MONTA, KSM01, KSM10)

#### **Packages**
- jupyterlab 2.2.9
- pandas 1.1.3
- xlrd 1.2.0
- geopandas 0.8.1
- bokeh 2.2.3
