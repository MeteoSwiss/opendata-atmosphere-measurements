[MeteoSwiss - Open Data](https://github.com/MeteoSwiss/opendata/blob/main/README.md) > [Understanding MeteoSwiss' Open Data products](https://github.com/MeteoSwiss/opendata/blob/main/README.md#understanding-meteoswiss-open-data-products) > B. Atmosphere Measurements

# B - Atmosphere Measurements
MeteoSwiss measures relevant data for weather forecasting and climate analysis in the [atmosphere](https://www.meteoswiss.admin.ch/weather/measurement-systems/atmosphere.html). The properties and composition of the atmosphere are studied using various instruments and methods, including but not limited to weather balloons, satellites, surface based remote sensing or commercial aircrafts.

The following measurements are available:

- B1 - [Radio soundings](#b1---radio-soundings)

The following measurements are planned to be made available for after the start of MeteoSwiss' Open Data provision:

- B2 - Raman-LIDAR for Meteorological Observation (RALMO)
- B3 - LIDAR Ceilometer CHM15K
- B4 - Ozone measurements - Total column (Dobson, Brewer)
- B5 - Ozone measurements - Profiles (O3 radio soundings, SOMORA)
- B6 - Swiss Alpine Climate Radiation Monitoring (SACRaM)

<br>

<!-- ### General information
All MeteoSwiss aerological stations have a name and an identfier consisting of three letters (e.g. `PAY` for [Payerne](https://www.meteoswiss.admin.ch/weather/weather-and-climate-from-a-to-z/weather-balloon.html). Data files use this station identifier (in lower case) in the file name throughout all directories. A list of all aerological station identfiers with station names, coordinates, height etc. can be found in the according 'station metadata' sections below. -->

---

## B1 - Radio soundings
MeteoSwiss performs [sounding](https://www.meteoswiss.admin.ch/weather/measurement-systems/atmosphere/radio-soundings.html) twice a day (`00:00 UTC` and `12:00 UTC`) from the sounding station in Payerne (station identifier `PAY`) using weather balloon radiosondes. The radiosondes measure temperature and humidity as well as its position and altitude using [GNSS](https://www.swisstopo.admin.ch/en/global-navigation-satellite-systems). Attached to a [weather balloon](https://www.meteoswiss.admin.ch/weather/weather-and-climate-from-a-to-z/weather-balloon.html) and carried high into the atmosphere, wind speed and direction as well as atmospheric pressure can further be derived. 

The data obtained in this way are of great importance for weather forecasts and climate research. The data collected during the radiosonde’s ascent are transmitted by radio to the receiving station in Payerne, where they are logged in the MeteoSwiss database. The results of the latest sounding are published  either as graphs ([emagrams](https://www.meteoswiss.admin.ch/services-and-publications/applications/radio-soundings.html#tab=radio-soundings-emagram)) or as [decoded data](https://www.meteoswiss.admin.ch/services-and-publications/applications/radio-soundings.html#tab=radio-soundings-decoded) files. 

### 1.1. Data granularity, update frequency, format and volume
The available file contains the data from the most recent sounding. The update frequency depends on the two soundings per day (at `00:00 UTC` and `12:00 UTC`).

Data format is [`CSV`](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#column-separators-decimal-dividers-and-missing-values) with an estimated volume of 0.02 MB per file.

See example data file for station PAY (set in lower case): [`ogd-radiosounding_pay_now.csv`](https://github.com/MeteoSwiss/publication-opendata/tree/main/data-atmosphere/radiosounding).

### 1.2. Parameter metadata and codes
See example [parameter metadata file](https://github.com/MeteoSwiss/publication-opendata/blob/main/data-atmosphere/radiosounding-PAY-metadata) incl. codes for 'Profile Type', 'Level Type' and 'Solar Radiation Correction'.

The productive version will provide a parameter metadata file with the file name: `ogd-radiosounding_meta_parameters.csv`.

<!-- ### Codes -->
<!-- ... -->

### 1.3. Station metadata
See example [station metadata file](https://data.geo.admin.ch/ch.meteoschweiz.messnetz-atmosphaere/ch.meteoschweiz.messnetz-atmosphaere_en.csv).

The productive version will provide a station metadata file with the file name: ogd-radiosounding_meta_stations.csv.

### 1.4. Data visualisation
See e.g. MeteoSwiss' [Emagrams](https://www.meteoswiss.admin.ch/services-and-publications/applications/radio-soundings.html#tab=radio-soundings-emagram).

<br>
