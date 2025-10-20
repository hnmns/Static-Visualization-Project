# US Native American Reservations, Socioeconomic Outcomes, and Gaming

Riley Kouns

## What is your current goal? Has it changed since the proposal?

I have completely switched topics to economic trends in US reservation populations. I switched from the domestic US steel supply chain to Native American reservation land census data, specifically as it correlates with registered gaming facilities. I now intend to show where reservations have been left behind on certain key economic measures, and whether there are any trends in those reservations that have improved the fastest in the last few decades. I hope to evaluate the average effect of gaming facility ownership on economic development at a micro level.

## Are there data challenges you are facing? Are you currently depending on mock data?

Gaming facility data like revenue is not public, so I instead relied on a pdf from the National Indian Gaming Commission for a list of all registered gaming facilities owned by Native American nations. I did some scripting and manual typo-fixing to crosswalk that casino ownership data to the Fed of MN's National Economic Trends (NET) data. The latter is a compilation of survey and census data for tribal lands and trusts. I was quite thorough about how I crosswalked the two data sets, but there are only gaming registry data for 2025, and the NET data is missing many years. Time series charts will be difficult or very limited.

## Describe each of the provided images with 2-3 sentences to give the context and how it relates to your goal.

The first chart below was the initial impetus of the whole project. American Indian and Alaska Native (AIAN) reservations are subject to a unique overlap of legal and political restrictions due to the ubiquitous jurisdiction of state and federal US government. As state governments began permitting Native American nations to establish their own gaming facilities for economic development, these nations had what seemed like a promising new revenue stream to lift communities out of historic poverty. I wanted to know the relationship between the number of gaming facilities owned by nations on a reservation and the classic economic measure of median household income. Did wealth "trickle out" to people from the economic development funds? I am working on how to make the LOESS look nicer and the federal median income more obvious.

![](/visualization/graphics/scatter_income_vs_facilitycount.svg)

The second chart is about the distribution of poverty rates on reservations over the years. I wanted to see if there is an obvious shift in the histogram of poverty since the passage of Native American gaming in the late 80s, either that reservations became less variable in wealth or that reservations actually experienced a reduced typical poverty rate overall. The blue median bars are supposed to be vertical dotted lines, but I couldn't figure out how to do that. I wonder how meaningful the median of a collection of rates really is.

![](/visualization/graphics/strip_poverty_vs_year.svg)

The third chart zooms in on a few northwestern states, which I decided partway through. I wanted to bring the study closer to home, and it was nicer for a bar chart to work with states that had far fewer reservations than, for example, California or Oklahoma. I really just wanted to highlight how the economic conditions on the reservation are unanimously less fortunate than the conditions overall. Ideally, I would be able to isolate off-reservation values rather than using state-wide values, but that is probably too much wrangling and would require more data searching.

![](/visualization//graphics/bar_state_facet_unemployment_vs_reservation.svg)

The fourth and fifth zoom in further on just Montana tribes to show the same idea as the third. I think it is helpful to have a "spaghetti" chart like the fifth, where the cloud of low-opacity lines shows the overall trend that holds true across reservations. This reinforces the idea from the third chart, but now it is evident across a number of critical economic outcomes that most people understand easily like education and income. I might be a little misleading by having lines that fill in the open spaces between data years, but a scatter plot would be so sparse as to not really look impactful. I think the linear interpolation is fair enough since no one is really meant to zoom in on specific values, just the overall trend of the two colors of line.

I am looking to pick couple of nations for comparison from the rank chart to see how their stories of economic development have looked qualitatively over the years. Maybe I can chart out the years of major events in their recent legal history. For a reason I do not yet know, the Fort Peck Reservation in the northeast jumped to the top of the home ownership rankings recently.

![](/visualization/graphics/rank_mt_houseownership_vs_year.svg)

![](/visualization/graphics/graphics/line_mt_outcome_facet_outcome_vs_year.svg)


The sixth shows what I somewhat expected about gaming facilities: That they de facto are not a silver bullet to economic issues. The first chart suggested it first, but there is perhaps only a higher upper bound on wealth measures associated with owning more gaming facilities. Reservations with many facilities and with no facilities seem to overlap in a co-located cloud of points. The impact of median income also obviously changes depending on the cost of living, which depends on the state. Maybe that is another facet to explore.

![](/visualization/graphics/scatter_bachelors_vs_income_byfacility.svg)

The seventh is a re-hash of the sixth, but using a measure that should not depend so much on the state where wealth is measured. The same statement from above about the upper bound on wealth measures seems to hold here. No silver bullets, apparently.

![](/visualization/graphics/scatter_youthpoverty_vs_income_byfacility.svg)

The eight was my attempt at checking the averages of the scatter plots in charts 6 and 7. Were the average economic outcomes in those two point clouds really that similar? What about over time rather than just in 2023? It turns out, reservations with no facilities were actually wealthier per capita in 2000, but just by a little. I wonder if it makes sense to aggregate incomes and populations this way.

![](/visualization/graphics/bar_year_facet_incomepercap_vs_facility.svg)

## What form do you envision your final narrative taking? (e.g. An article incorporating the images? A poster? An infographic?)

Since there are so many "outliers" between the two data sets that I used, this narrative absolutely requires an article surrounding it. A poster would have too many crowded footnotes and asides to explain why some data on a nation can't be used for a certain year (e.g. only 10 observations of a very small nation), or why a select few nations appear very wealth (e.g. Shakopee Mdewakanton).

It would also be far too easy to treat hundreds of different peoples as just "Native Americans" if I were to put this all in a poster. The sparse nature of these data (in both time and in missing values) makes it difficult to paint very detailed pictures of individual nations, so I am trying my best to not just aggregate the story into natives versus non-natives. Instead, I would like to take the time to highlight success stories and the nations most in need of attention. For that, I will need to put the visualizations in the context of an article.