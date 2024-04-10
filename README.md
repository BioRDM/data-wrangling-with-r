# Data wrangling with R

Showcase notebooks for data cleaning with R inspired by our real data curation work for the project about monitoring COVID virus levels in wastewater around Scotland [see project page](https://covid-ww-scotland.github.io/).

The notebooks capture the typical workflows for data curation in biomedical data (probably also suitable any other discipline where data are entered manually into spreadsheets).

The folder structure is (`out` and `data` are not under version control):
```
- data - curated input data
- out - generated different forms of data 
- raw_data - input data (COVID prevalence, sites coordinates and population)
- src - RMarkdown notebooks for data cleaning
```

* [data-wrangling-01](src/data-wrangling-01.Rmd) - renaming columns name to follow consistent naming convention and follow tidy tables recommendations

* [data-wrangling-02](src/data-wrangling-02.Rmd) - finding misspelled entries, checking data sanity (number of records per site, negative values etc), replace misspelled entries, changing data format to ISO, adding missing entries

* [data-wrangling-03](src/data-wrangling-03.Rmd) - preparing data from a source to join(prevalence with sites locations)


* [data-wrangling-04](src/data-wrangling-04.Rmd) - curating population data


* [data-wrangling-05](src/data-wrangling-05.Rmd) - joining the two sites tables (populatin and coordination) into one


* [data-wrangling-06](src/data-wrangling-06.Rmd) - merging the main covid data with coordinates and population (denormalization of the data)


* [data-wrangling-07](src/data-wrangling-07.Rmd) - creation of timeseries data, *wide* table with a column for each date


* [data-wrangling-08](src/data-wrangling-08.Rmd) - creation of aggregated timeseries data (per week number)


* [data-wrangling-09](src/data-wrangling-09.Rmd) - preparation of breakpoints for a color scale to be used with a heatmap


* [data-wrangling-10](src/data-wrangling-10.Rmd) - generating heatmaps with virus levels per date





