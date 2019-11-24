This is a template you can use for your final projects (as well other projects where you need to post replication code.) Fill in each section with information on your own project.

## Short Description

Give a short, 1-2 paragraph description of your project. Focus on the code, not the theoretical / substantive side of things. 

## Dependencies

List what software your code depends on, as well as version numbers, like so:.

1. R, 3.6.1

In your scripts, includes commands that `require()` packages.

## Files

List all files (other than `README.md` and `Final-Project.RProj`) contained in the repo, along with a brief description of each one, like so:

#### /

1. Narrative.Rmd: Provides a 3-5 page narrative of the project, main challenges, solutions, and results.
2. Narrative.pdf: A knitted pdf of 00_Narrative.Rmd. 
3. Slides.XXX: Your lightning talk slides, in whatever format you prefer.

#### Code/
1. 01_collect-nyt.R: Collects data from New York Times API and exports data to the file nyt.csv
2. 02_merge-data.R: Loads, cleans, and merges the raw Polity and NYT datasets into the Analysis Dataset.
3. 03_analysis.R: Conducts descriptive analysis of the data, producing the tables and visualizations found in the Results directory.

#### Data/

1. polity.csv: The PolityVI dataset, available here: http://www.systemicpeace.org/inscrdata.html
2. nyt.csv: Contains data from the New York Times API collected via collect-nyt.ipynb . Includes information on all articles containing the term "Programmer Cat", 1980-2010.
3. analysis-dataset.csv: The final Analysis Dataset derived from the raw data above. It includes country-year values for all UN countries 1980-2010, with observations for the following variables: 
    - *ccode*: Correlates of War numeric code for country observation
    - *year*: Year of observation
    - *polity*: PolityVI score
    - *nyt*: Number of New York Times articles about "Programmer Cat"

#### Results/

1. coverage-over-time.jpeg: Graphs the number of articles about each region over time.
2. regression-table.txt: Summarizes the results of OLS regression, modelling *nyt* on a number of covariates.

## More Information

Include any other details you think your user might need to reproduce your results. You may also include other information such as your contact information, credits, etc.

