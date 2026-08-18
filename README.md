# Emergency Food Network Service Demand & Utilization Analysis

Applied analysis of multi-year administrative data from **Emergency Food Network (EFN)** examining how service activity, repeat utilization, food distribution, and client composition changed across the partner network from 2014–2024.

The project emphasizes **data validation, descriptive analysis, operational interpretation, and careful treatment of data limitations**. A limited time-series extension is included as a secondary exercise to evaluate what the short annual series can reasonably support for planning purposes.

## Project Overview

The analysis examines recorded activity across EFN service units to better understand:

- Changes in service reach and total activity over time
- Repeat utilization and service intensity
- Food distribution patterns and capacity
- Demographic composition of clients served
- Variation across geographic and program-level service units
- The extent to which historical activity supports a cautious forecasting baseline

The primary goal is descriptive rather than causal. The data measure activity within the observed EFN partner system and should not be interpreted as direct measures of underlying community food insecurity or unmet need.

## Key Findings

- Total service activity increased substantially over the observed period, particularly after 2020.
- Growth in total service encounters outpaced growth in unique clients, indicating increased **repeat utilization** over time.
- Average activity per service unit also increased, suggesting that system growth was not driven solely by expansion in network coverage.
- Service volume and food distribution varied meaningfully across service units, demonstrating substantial heterogeneity in operational scale and utilization.
- The post-2020 period shows considerably greater instability than earlier years, limiting the reliability of simple trend extrapolation.
- The available annual series does **not** support high-confidence forecasting. The time-series component is therefore presented as a conservative planning baseline rather than the central contribution of the project.

## Data Structure & Validation

The dataset contains annual administrative records at the **service unit–year** level from 2014–2024.

Service-unit identifiers include both geographic ZIP codes and program-level identifiers, creating an **unbalanced panel** as service units enter or exit the observed network over time.

Before conducting the analysis, I:

- Defined the unit of observation and analytical scope
- Distinguished geographic ZIP-coded records from program-level service identifiers
- Validated relationships among unique clients, repeat visits, and total service encounters
- Verified key accounting identities across the dataset
- Investigated zero values and potential reporting inconsistencies
- Documented the appropriate interpretation and limitations of food-distribution measures

These checks established the analytical foundation for the subsequent descriptive and time-series work.

## Methods

### Descriptive & Operational Analysis

- Data validation and consistency checks
- Exploratory data analysis
- Longitudinal trend analysis
- Service reach and utilization analysis
- Repeat-visit intensity
- Food distribution analysis
- Demographic composition
- Cross-service-unit comparisons

### Limited Time-Series Extension

The project also evaluates whether aggregate annual service activity supports a defensible univariate forecasting exercise.

Because the series contains only **11 annual observations** and becomes substantially more unstable after 2020, the forecasting component emphasizes methodological restraint rather than predictive complexity.

The extension includes:

- Aggregate annual time-series construction
- Stationarity assessment
- ADF and KPSS testing
- Transformation and differencing
- Parsimonious model comparison
- Residual diagnostics
- Conservative baseline projections with explicit uncertainty

The resulting forecasts should be interpreted as exploratory planning baselines, not precise predictions of future demand.

## Project Files

### [Executive Summary](./reports/01_EFN_Executive_Summary.pdf)

Concise overview of the project, principal findings, limitations, and interpretation.

### [Data Structure, Definitions & Validation](./reports/03_Data_Structure_Definitions_and_Validation.pdf)

Documents the data-generating process, unit of observation, variable definitions, accounting checks, zero-value diagnostics, and analytical limitations.

### Exploratory Data Analysis

Core descriptive analysis of service reach, repeat utilization, food distribution, demographic composition, and variation across service units.

### [Limited Time-Series Extension](./reports/05_Limited_Time_Series_Extension.pdf)

Evaluates the time-series properties of aggregate service activity and develops a deliberately conservative forecasting baseline under substantial data limitations.

## Tools

**Python** · **pandas** · **NumPy** · **Matplotlib** · **statsmodels** · **scikit-learn** · **Jupyter Notebook**

## Analytical Limitations

The dataset records observed service activity within EFN's partner network rather than the full population experiencing food insecurity. Changes in partner participation, service coverage, program structure, and reporting may also affect observed trends.

The forecasting extension is particularly constrained by the short annual series and the structural instability evident after 2020. For that reason, uncertainty and analytical limits are emphasized throughout the project rather than presenting the projections as high-confidence forecasts.

## Author

**Chad Asindraza**  
M.A. Economics  
University of Nevada, Las Vegas
