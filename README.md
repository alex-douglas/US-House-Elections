# 2016 U.S. House of Representatives Elections

### Goal

The goal of this project is to see if we can predict the margin of victory in election results for the U.S. House of Representatives based on biographical information about the winning candidates.

### Reasoning

I would think that biographical information about individual politicans should have no impact on their margin of victory. Other variables are likely to drown out any influence marriage, children, or education might have on the outcome of the elections. However, the goal of this project was to develop our web scrapping skills in addition to learning about linear regression, so I am gathering biographical information for politicans since this data is available from their Wikipedia pages.

I will also get the margin of victory for each district in the 2014 elections, as a control variable to compare against the biographical variables. I would expect this to be a massive predictor of election results in 2016, since districts tend to vote similarly from year to year, and gerrymandering has made this feature of House elections more and more true. I will also get the date they assumed office and their party, which aren't biographical variables, and I would expect these two to potentially influence the margin of victory, though mabye not as much as the margin of victory in 2014.

### Project Process

1. Scrape the [wikipedia page](https://en.wikipedia.org/wiki/Current_members_of_the_United_States_House_of_Representatives) of the current list of Representatives, which will give their names, districts, and links to their specific Wikipedia pages.
2. Scrape the individual Wikipedia pages for each Representative, and get the following variables if available:
    - date assumed office
    - birthday
    - number of children
    - marital status
    - party
    - education (type of degree)
    - occupation
    - gender
3. Scrape the [2014 margins](https://ballotpedia.org/Margin_of_victory_analysis_for_the_2014_congressional_elections) from the ballotpedia.org website.
4. Scrape the [2016 margins](https://ballotpedia.org/United_States_House_of_Representatives_elections,_2016) from the ballotpedia.org website.
5. Combine all the collected data into one dataframe.
6. Clean the data.
6. Explore the data with linear regression techniques and determine the best model to predict the 2016 margins.

See 'Project 2 Notebook - Alex Douglas' in the [Jupyter Notebooks folder](Jupyter%20Notebooks/) for a step-by-step walkthrough of the project.
