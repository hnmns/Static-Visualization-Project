# Riley Kouns

## Description

I want to visualize iron ore (or metallic ore in general) freight movements domestic to the USA, broken down by transit mode and year. Ultimately, I intend to highlight key origin-destination pairs in the domestic US steel production supply chain, singling out bottlenecks and regions that warrant further transportation infrastructure investment.

## Data Sources

### Data Source 1: Federal Highway Administration's Freight Analysis Framework (FAF)

URL: [FAF Data Tabulation Tool](https://ops.fhwa.dot.gov/freight/freight_analysis/faf/)

Size: 18460 rows, 8 columns (after wrangling)

These origin-destination pair readings for freight go back as far as 2017 and include estimates as far forward as 2050. By default, the data come in wide format with year and freight measure encoded in columns. I selected 2024 (the most recent year with data available), 2019 (a round five years ago, also before the full set-in of pandemic economic disruptions), and 2030 (the soonest year they provide for predictions). The estimated year has a low and a high prediction.

### Data Source 2: US Army Corp of Engineers' Waterway Locks

URL: [National Transportation Atlas Database (Data.gov)](https://catalog.data.gov/dataset/waterway-locks1)

Size: 234 rows, 46 columns

This is a geospatial data set that maps locks along the mainland US' inland waterways. The data set includes some information on which river the lock is located on, the lock's dimensions, and its nearest city, but most important to this project are simply the coordinates.

## Questions

1. How can I best visualize origin-destination pairs that aren't linear (e.g. the inland waterway between two states follows a zig-zagging river)? I think it would be cool to highlight the actual route taken by freight, but with many O-D pairs and lots of geography, I can see how this could get convoluted quickly.
2. Is it necessary to access both of our data sources? My second data source has (necessarily) far fewer observations, but could be a helpful supplement to the first data source, especially to highlight chokepoints in shipping.