[MeteoSwiss - Open Data](https://github.com/MeteoSwiss/opendata/blob/main/README.md) > [Understanding MeteoSwiss' Open Data products](https://github.com/MeteoSwiss/opendata/blob/main/README.md#understanding-meteoswiss-open-data-products) > B. Atmosphere Measurements

# B. Atmosphere Measurements
MeteoSwiss obtains relevant data for weather forecasting and climate analysis from the [atmosphere](https://www.meteoswiss.admin.ch/weather/measurement-systems/atmosphere.html). The properties and composition of the atmosphere are studied using various instruments and methods, including weather balloons, satellites and laser equipment. Weather radar stations play an important role, as they record precipitation and thunderstorms throughout Switzerland in real time.

The following measurements are available:

1. [Radio soundings](#1-radio-soundings) :yellow_circle: *in review by MDA*

The following measurements are planned to be made available:

- Raman-LIDAR for Meteorological Observation (RALMO) :large_blue_circle: *planned for after go-live*
- LIDAR Ceilometer CHM15K :large_blue_circle: *planned for after go-live*
- Ozone measurements
   - Ground-based: Dobson, Brewer :large_blue_circle: *planned for after go-live*
   - Atmosphere: O3 radio soundings, SOMORA :large_blue_circle: *planned for after go-live*
- Swiss Alpine Climate Radiation Monitoring (SACRaM) :large_blue_circle: *planned for after go-live*

### General information
All MeteoSwiss aerological stations have a name and an identfier consisting of three letters (e.g. `PAY` for [Payerne](https://www.meteoswiss.admin.ch/weather/weather-and-climate-from-a-to-z/weather-balloon.html). Data files use this station identifier in the file name throughout all directories. A list of all aerological station identfiers with station names, coordinates, height etc. can be found in the according 'station metadata' sections below.

---

## 1. Radio soundings
MeteoSwiss performs [sounding](https://www.meteoswiss.admin.ch/weather/measurement-systems/atmosphere/radio-soundings.html) twice a day (`00:00 UTC` and `12:00 UTC`) from the sounding station in Payerne (station identifier `PAY`) using weather balloon radiosondes. The radiosondes measure air pressure, temperature and humidity. Attached to a [weather balloon](https://www.meteoswiss.admin.ch/weather/weather-and-climate-from-a-to-z/weather-balloon.html) and carried high into the atmosphere, the radiosonde also records the exact position, allowing altitude, wind speed and direction to be determined. 

The data obtained in this way are of great importance for weather forecasts and climate research. The data collected during the radiosonde’s ascent are transmitted by radio to the receiving station in Payerne, where they are logged in the MeteoSwiss database. The results of the latest sounding are published  either as graphs ([emagrams](https://www.meteoswiss.admin.ch/services-and-publications/applications/radio-soundings.html#tab=radio-soundings-emagram)) or as [decoded data](https://www.meteoswiss.admin.ch/services-and-publications/applications/radio-soundings.html#tab=radio-soundings-decoded) files. 

### Data granularity, update frequency, format and volume
The available file contains the data from the most recent sounding. The update frequency depends on the two soundings per day (at `00:00 UTC` and `12:00 UTC`).

Data format is [`CSV`](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#column-separators-decimal-dividers-and-missing-values) with an estimated volume of 0.02 MB per file.

See (example!) data file: [`ogd-radiosounding_PAY_now.csv`](https://github.com/MeteoSwiss/publication-opendata/tree/main/data-atmosphere/radiosounding).

### Parameter metadata and codes
See (example!) [parameter metadata file](https://github.com/MeteoSwiss/publication-opendata/blob/main/data-atmosphere/radiosounding-PAY-metadata) incl. codes for 'Profile Type', 'Level Type' and 'Solar Radiation Correction'.

The productive version will provide a parameter metadata file with the file name: `ogd-radiosounding_meta_parameters.csv`.

<!-- ### Codes -->
<!-- ... -->

### Station metadata
See (example!) [station metadata file](https://data.geo.admin.ch/ch.meteoschweiz.messnetz-atmosphaere/ch.meteoschweiz.messnetz-atmosphaere_en.csv).

The productive version will provide a station metadata file with the file name: ogd-radiosounding_meta_stations.csv.

### Data visualisation
See e.g. MeteoSwiss' [Emagrams](https://www.meteoswiss.admin.ch/services-and-publications/applications/radio-soundings.html#tab=radio-soundings-emagram).
