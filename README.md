# Remote sEnsing based multi-sensor Spatio-tEmporal fusion aided ReserVOIR MAPPing framEwoRk (RESERVOIR MAPPER)
**Framework Overview**
•	Core Objective: Designed to generate dense and temporally continuous reservoir water spread time-series.
•	Sensor Integration: Integrates high-resolution optical (Sentinel-2) and Synthetic Aperture Radar (Sentinel-1) datasets to overcome the limitations of cloud cover.
•	Advanced Fusion: Utilizes spatial fusion techniques where cloud-contaminated optical pixels are replaced by data from the temporally nearest SAR water scene.
•	Platform: Built entirely on the Google Earth Engine (GEE) platform, leveraging its high-performance cloud computing and extensive data catalog.
•	Methodology: Produces independent water masks using adaptive Otsu thresholding for both optical water indices and SAR polarization data.


**Implementation Instructions**
•	Setup: Paste the "Reservoir_Mapper" code into the Google Earth Engine Code Editor, Input the lake geometry using a buffered boundary to ensure the area covers the maximum potential water spread and seasonal fluctuations. and Run it.
•	Note on Large Data Extraction: To access the water spread time-series for longer time periods (e.g., several years), go to the Tasks panel of the Google Earth Engine code editor and Export the CSV output to your Google Drive. This method bypasses the "Capacity Exceeded" or "Computation Timed Out" warnings associated with on-the-fly console printing.

**Acknowledgments**
The authors gratefully acknowledge the European Space Agency (ESA) for providing open-access Sentinel-1 and Sentinel-2 satellite data and the U.S. Geological Survey (USGS) for the Shuttle Radar Topography Mission (SRTM) elevation dataset. All datasets were accessed and processed via the Google Earth Engine platform.
