# Remote sEnsing based multi-sensor Spatio-tEmporal fusion aided ReserVOIR MAPPing framEwoRk (RESERVOIR MAPPER)

## Framework Overview
* **Scope & Objective:** This framework can be used across diverse climatic and geographic regions worldwide to generate dense and temporally continuous reservoir water spread time-series.
* **Multi-Sensor Fusion Strategy:** Integrates high-resolution optical (Sentinel-2) and Synthetic Aperture Radar (Sentinel-1) datasets to overcome the limitations of cloud cover.
      *  Utilizes spatial fusion techniques where cloud-contaminated optical pixels are replaced by data from the temporally nearest SAR water scene.
* **Platform:** Built entirely on the Google Earth Engine (GEE) platform, leveraging its high-performance cloud computing and extensive data catalog.
* **Reference:** For more details refer our article titled "Remote sEnsing based multi-sensor Spatio-tEmporal fusion aided ReserVOIR MAPPing framEwoRk (RESERVOIR MAPPER)" by Shekhar and Ramsankaran (2026) Remote Sens. Appl. Soc. Environ. [DOI: 10.1016/j.rsase.2026.102054).

---

## Implementation Instructions
* **Setup:** Paste the "Reservoir_Mapper" code into the Google Earth Engine Code Editor.
* **Geometry Input:** Input the lake geometry using a buffered boundary to ensure the area covers the maximum potential water spread and seasonal fluctuations.
    * **Option A (Manual Digitization):** Use the GEE drawing tools to create a new polygon layer around the reservoir directly on the map.
    * **Option B (Shapefile Import):** Go to the GEE 'Assets' tab, click 'New' > 'Shape files', upload your zipped shapefile component files (.shp, .shx, .dbf, .prj), and import it into your script.
* **Execution:** Run the code within the GEE platform.
* **Note on Large Data Extraction:**
* **Data Export:**  To access the water spread time-series for longer time periods (e.g., several years), Export the CSV output to your Google Drive.
    * **Steps:** Locate the 'Tasks' tab, click the 'Run' button next to the task, configure your preferred Drive folder path in the popup window, and click 'Run' again to begin the background export.
    * **Note:** This method bypasses the "Capacity Exceeded" or "Computation Timed Out" warnings during processing on GEE.

---

**Acknowledgments:** The authors gratefully acknowledge the European Space Agency (ESA) for providing open-access Sentinel-1 and Sentinel-2 satellite data and the U.S. Geological Survey (USGS) for the Shuttle Radar Topography Mission (SRTM) elevation dataset. All datasets were accessed and processed via the Google Earth Engine platform. 

---

**Credits:** Developed by Sparsh Shekar, research scholar from the Hydro-Remote Sensing Applications (H-RSA) Group, Department of Civil Engineering, Indian Institute of Technology (IIT) Bombay, Mumbai
