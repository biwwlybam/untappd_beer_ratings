# Scraping Untappd Beer Scores

The goal of this project is to scrape Untappd for all of a brewery's beer scores and store them in a dataframe. The idea is that this could be done at a set time interval (daily, weekly, monthly, etc) in order to have data showing how different brands' ratings have changed over time.

This would be useful for a brewery that wants to track their core brands' scores to make sure they are consistently hitting quality standards and meeting or exceeding consumer expectations. A downward trend in score would indicate that the brand needs attention. Likewise, it would be useful for comparing the scores of one-off beers, maybe of similar style, to see what has been successful and be able to deduce the reason. The resulting dataframe from this code allows for grouping by style.

## Creating the dataframe

We will use `create_df.ipynb` first to create our original dataframe. This will contain all beer names, styles, and scores available on Untappd for a specific brewery. I have used Burial Beer in Asheville, NC as an example, but the only change that would need to be made is updating the urls in the `driver.get()` methods. The other change that each specific user of these files will need to make is inputting their own username and password into those labeled fields in the code.

## Updating the dataframe

This file is still in progress, but the goal is to create a new dataframe at a later date than the original, and join it to add new beers to the end of the dataframe and add a new column with this later date's scores.
