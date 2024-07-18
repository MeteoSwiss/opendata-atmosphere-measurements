[MeteoSwiss - Open Data](https://github.com/MeteoSwiss/opendata/blob/main/README.md) > [Understanding MeteoSwiss' Open Data products](https://github.com/MeteoSwiss/opendata/blob/main/README.md#understanding-meteoswiss-open-data-products) > B. Atmosphere Measurements

# B. Atmosphere Measurements
...

1. [Radio soundings](#1-radio-soundings)

---

## 1. Radio soundings
MeteoSwiss performs [sounding](https://www.meteoswiss.admin.ch/weather/measurement-systems/atmosphere/radio-soundings.html) twice a day from the sounding station in Payerne (station identifier `PAY`) using weather balloon radiosondes. The radiosondes measure air pressure, temperature and humidity. Attached to a [weather balloon](https://www.meteoswiss.admin.ch/weather/weather-and-climate-from-a-to-z/weather-balloon.html) and carried high into the atmosphere, the radiosonde also records the exact position, allowing altitude, wind speed and direction to be determined. 

The data obtained in this way are of great importance for weather forecasts and climate research. The data collected during the radiosonde’s ascent are transmitted by radio to the receiving station in Payerne, where they are logged in the MeteoSwiss database. The results of the latest soundings are published  either as graphs ([emagrams](https://www.meteoswiss.admin.ch/services-and-publications/applications/radio-soundings.html#tab=radio-soundings-emagram)) or as [decoded data](https://www.meteoswiss.admin.ch/services-and-publications/applications/radio-soundings.html#tab=radio-soundings-decoded) files. 

### Data granularity, update frequency, format and volume
There are files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity) `...` and [update frequency](https://github.com/MeteoSwiss/opendata-download/blob/main/README.md#update-frequency) ... (`now`).

Data format is [`CSV`](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#column-separators-decimal-dividers-and-missing-values) with an estimated volume of 0.02 MB per file.

See (example!) data files: [`ogd-radiosounding_PAY_now.csv`](https://github.com/MeteoSwiss/publication-opendata/tree/main/data-atmosphere/radiosounding).

### Parameter metadata
See (example!) parameter metadata files of [data granularity](https://github.com/MeteoSwiss/opendata-download?tab=readme-ov-file#data-granularity): [`...`](...) and [`...`](...).

<!-- ### Codes -->
<!-- ... -->

### Station metadata
See (example!) [station metadata file](...).

### Data visualisation
See e.g. MeteoSwiss' [...](...).
