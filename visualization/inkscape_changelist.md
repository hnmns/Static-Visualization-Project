
General notes
* Some areas split into subdivisions (geoname_datayear) in the 1990s, so drop their 1990s values for now
    * Knik ANVSA
    * Navajo Nation Reservation and Off-Reservation Trust Land
        * Merged 4 regions into 1 after 1990
    * Tohono O'odham Nation Reservation and Off-Reservation Trust Land
    * Knik ANVSA
    * Bois Forte Reservation and Off-Reservation Trust Land
    * Mille Lacs Reservation and Off-Reservation Trust Land
        * Also split in 2000
* Reservations were attributed to states based on where their nations' gaming facilities were located
    * This could lead to conflicts if two nations on the same reservations open facilities in different states' borders (Navajo, Colorado River Reservations both have land within multiple states)


1. Median income vs. number of gaming facilities scatter plot
    * Remove states, federal
    * Remove points on LOESS (g1235)? Only if loess has shape encoding
    * Change AIANa for American Indian / Alaska Native alone
    * Add legend annotation "Trendlines (for each population) in matching colors"
        * Add legend white background 0.5 opacity. Why is it gone after saving svg?
    * Footnote about dropping 
        * (NOT Shakopee Mdewakanton Sioux) 
        * Redding Rancheria (outlier, small obs)
        * Sulphur Bank Rancheria (N=6)
        * Klamath only has about 26 (+/- 17) households in 2023!
        * Quechan Indian Tribe/CA dropped, conflicted with Quechan Tribe of the Fort Yuma Indian Reservation, CA and AZ (duplicate entry, clerical holdover of renaming)
    * Give Shakopee annotation text a low-opacity white background
        * Remove "Community?"

2. Poverty levels over time (strip plot)
    * Clear instances of 100% poverty rate, often associated with community survey years having extremely small sample sizes (e.g. N=15 when Havasupai Reservation had 100% poverty in 2018)

3. Native Nation vs. State unemployment rates (bar chart)
    * Note that Snoqualmie in WA are missing unemployment data
    * I do not have state data on any nations that do not own a facility
        * Really, this study is geographically sparse in terms of facility location
        * I will just manually fill in missing states for the purpose of this chart
    * **Inkscape**
        * Shift Washington facet and legend upward to close some of the negative space

4. Rank chart of housing in MT reservations
    * Add shadow or outline to nation names

## Other issues
* Drop Oklahoma statistical areas (and Navajo Nation?)
* Many small nations -> Many small sample sizes
* Starting in 2000, ACS responses allowed self-identification as more than one race