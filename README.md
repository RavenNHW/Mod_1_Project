# How to Make a Hit
**Maximizing Movie Revenue**

## Overview:
Microsoft has hired our team to help them enter the movie production industry.  They currently have no industry knowledge and need information on which movies are currently doing well at the box office.  We aim to give them actionable insights into what kind of movies they should produce in order to maximize their revenue.

**The Questions:**
* How does genre affect revenue?
* What is the optimal movie length in order to maximize revenue?
* Who are the top generators of revenue?  Do certain actors or directors have strong track records?

### ReadME Navigation

[Data](https://github.com/RavenNHW/Mod_1_Project#data) -
[Results](https://github.com/RavenNHW/Mod_1_Project#results) - 
[Recommendations](https://github.com/RavenNHW/Mod_1_Project#recommendations) - 
[Limitations & Next Steps](https://github.com/RavenNHW/Mod_1_Project#limitations-and-next-steps) - 
[Reproduction Instructions](https://github.com/RavenNHW/Mod_1_Project#reproduction-instructions) -
[Project Information](https://github.com/RavenNHW/Mod_1_Project#project-information) -


## Data
**Sources:**
Data for movie genre, runtime, name, and production crew was gathered from [IMDB](www.imdb.com).
Revenue data was gathered from [BoxOfficeMojo](https://data.world/eliasdabbas/boxofficemojo-alltime-domestic-data) by a third party.

**The Dataset:**
Our dataset contains 3200 movies produced between 2010 and 2019.  Each movie has data on genre, lifetime revenue, production year, and runtime.  Each movie can be counted in multiple different genres.  Analysis focuses on feature-length films, so movies under 60 minutes were not considered.  Supplementary data includes important cast and crew members.

All revenue data analyzed in this project shows gross domestic revenue.  


## Results
**Top Actors**

![](https://github.com/RavenNHW/Mod_1_Project/blob/master/Images/People_Actor_1.png)

The top 10 actors in terms of median revenue all have strong track records of generating high revenue films.  Many of these actors are featured in successful franchises like Star Wars, The Avengers, The Hobbit, and Fast & Furious.

**Top Directors**

![](https://github.com/RavenNHW/Mod_1_Project/blob/master/Images/People_Director_1.png)

These findings are similar to the top actors.  Many of the directors with the highest earnings are linked to successful movie franchises.

**Runtime Analysis**

![](https://github.com/RavenNHW/Mod_1_Project/blob/master/Images/Runtime_1.png)

Movies between 1:52 and 2:05 earn higher revenues on average.  Movies are grouped into bins, each of which contain about 500 films.  

Legend:
* Very Short: 1:00-1:29
* Short: 1:30-1:35
* Medium: 1:36-1:42
* Medium-Long: 1:43-1:51
* Long: 1:52-2:05
* Very Long: >2:05


**Genre Trends**

![](https://github.com/RavenNHW/Mod_1_Project/blob/master/Images/Genre_Process_2.png)

Median revenues are consistently high for Adventure and Sci-Fi movies.  These genres are trending up in recent years.

**Adventure & Sci-Fi**

![](https://github.com/RavenNHW/Mod_1_Project/blob/master/Images/Genre_Process_3.png)

Sci-Fi movies have a wider variance in revenues.  This indicates that they are riskier, but have higher potential revenue.  Adventure movies generate more stable revenues.


## Recommendations
* Hire top directors and writers.
* Produce movies that are about 2 hours in length.
* Create movies that fit into the Adventure and Sci-Fi genres.

## Limitations and Next Steps
**Limitations:**
* Due to unreliability of production budget data, movie profit and production cost are not taken into account.
* Analysis focuses only on domestic box office.
* Revenue data is not adjusted for inflation.

**Next Steps:**

With further analysis, more insightful recommendations could be delivered.  Questions for additional analysis are as follows:

* What are the source materials for the most popular movie series?  What source materials can Microsoft license for movie production?
* Who is the most skilled at making each genre of movie?
* Do certain key principals work well together?
* How does a movie's opening weekend affect its lifetime revenue?

**Further Information:**
Please review the [jupyter notebook](https://github.com/RavenNHW/Mod_1_Project/blob/master/Data%20Processing/Data_Analysis.ipynb) and [presentation](https://github.com/RavenNHW/Mod_1_Project/blob/master/presentation.pdf) located in this repository.

## Reproduction Instructions
1. Download IMDB and BoxOfficeMojo [source data](https://github.com/RavenNHW/Mod_1_Project#data).
2. Run [Generate_CSVs](https://github.com/RavenNHW/Mod_1_Project/blob/master/Data%20Processing/Generate_CSVs.ipynb).
2. Run [Creating_Master_Table](https://github.com/RavenNHW/Mod_1_Project/blob/master/Data%20Processing/Generate_Master_Table.ipynb).
3. Run [Create_People_Master](https://github.com/RavenNHW/Mod_1_Project/blob/master/Data%20Processing/Generate_People_Table.ipynb).
4. Run main [Jupyter Notebook](https://github.com/RavenNHW/Mod_1_Project/blob/master/Data%20Processing/Data_Analysis.ipynb).




## Project Information
**Contributors:** [Raven Welch](https://github.com/RavenNHW), [Jim Fay](https://github.com/jrf6xh)

**Languages:** Python

**Libraries:** pandas, matplotlib, seaborn

**Duration:** June 15 - June 18, 2020

**Last Update:** June 18, 2020