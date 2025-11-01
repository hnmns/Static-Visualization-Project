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
    * Give Shakopee annotation text a low-opacity white background
        * Remove "Community?"

2. Poverty levels over time (strip plot)
    * Blue median datum: `mark_tick()` does not support `strokeDash` because ticks are *rectangles*, not lines
        * Check if Inkscape allows a dotted stroke


## Other issues
* Drop Oklahoma statistical areas (and Navajo Nation?)
* Many small nations -> Many small sample sizes
* Starting in 2000, ACS responses allowed self-identification as more than one race