# Meteorological Drought Analysis using SPI-3 and SPI-6

This project analyzes meteorological drought conditions over Peninsular India using the Standardized Precipitation Index (SPI). The analysis uses monthly precipitation data from January 2000 to September 2024 to identify drought events and compare drought behavior at 3-month and 6-month timescales.

The spatially averaged monthly precipitation was first converted into a continuous rainfall time series. Three-month and six-month rolling rainfall totals were then calculated for SPI-3 and SPI-6. A Gamma probability distribution was fitted to the rainfall data, and the resulting cumulative probabilities were transformed into standardized normal values to obtain SPI.

Drought events were identified using SPI < 0. The analysis then characterized the detected events based on their frequency, duration, severity, and intensity.

## Key Results

- SPI-3 identified **24 drought events**, while SPI-6 identified **25 events**.
- Average drought duration was **6.04 months for SPI-3** and **5.24 months for SPI-6**.
- Average drought intensity was **-0.89 for SPI-3** and **-0.96 for SPI-6**.
- Average severity was **-5.38 for SPI-3** and **-5.12 for SPI-6**.

## SPI-3 vs SPI-6

SPI-3 responds more quickly to short-term rainfall fluctuations and captures shorter-term changes in drought conditions. SPI-6 provides a smoother response to rainfall variability and represents more sustained drought conditions. Comparing both timescales helps provide a broader view of meteorological drought behavior.

## Workflow

1. Prepare monthly precipitation data for Peninsular India.
2. Calculate spatially averaged monthly rainfall.
3. Generate 3-month and 6-month rolling rainfall totals.
4. Fit the rainfall data to a Gamma distribution.
5. Convert cumulative probabilities to SPI values.
6. Identify drought events using SPI < 0.
7. Calculate drought frequency, duration, severity, and intensity.
8. Compare SPI-3 and SPI-6 drought characteristics.

## Data & Tools

- Monthly precipitation data (2000–2024)
- Python
- NumPy
- Pandas
- SciPy
- Matplotlib
- NetCDF data processing

## Repository Contents

The repository contains the analysis notebook, assignment report used for the SPI-3 and SPI-6 drought analysis.
