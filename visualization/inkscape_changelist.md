
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
    * Blue median datum: `mark_tick()` does not support `strokeDash` because ticks are *rectangles*, not lines
        * Check if Inkscape allows a dotted stroke


3. Native Nation vs. State unemployment rates (bar chart)
    * Note that Snoqualmie in WA are missing unemployment data

## Other issues
* Drop Oklahoma statistical areas (and Navajo Nation?)
* Many small nations -> Many small sample sizes
* Starting in 2000, ACS responses allowed self-identification as more than one race