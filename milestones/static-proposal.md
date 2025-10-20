# Riley Kouns

## Description

I want to prepare a suite of visualizations comparing socioeconomic outcomes with gaming facility ownership in nations on Native American reservations.

## Data Sources

### Data Source 1: Fed of Minneapolis

From the Center for Indian Country Development.

Some critical notes on these data:
* Not every nation has a reservation. Some nations only have land held in trust by the federal government of the United states (e.g. Kaw Nation of Oklahoma). You may see something like "Kaw OTSA," which is only a statistical area, but not land owned exclusively by the Kaw Nation. Unless I later find that these regions do not meaningfully encompass these nations, I will treat them similarly, as the nations are still based in these areas as far as I have verified.
* Some federally recognized tribes are in the same statistical area, especially in Oklahoma (e.g. Creek OTSA encompasses Thlopthlocco Tribal Town)

URL: [Native Economic Trends](https://www.minneapolisfed.org/indiancountry/resources/native-economic-trends)

Size: (5074, 75)


### Data Source 2: National Indian Gaming Commission

This is a messy pdf with a no-outline table that bleeds over lines frequently. I will extract the count of gaming facilities by nation, their address, and their facility class.

URL: [NIGC Gaming Facilities](https://www.nigc.gov/map/)

Size: (774, 7)
