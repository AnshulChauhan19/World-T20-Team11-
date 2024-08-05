<div style="border: 2px solid black; text-align: center; padding: 15px; border-radius: 5px; background-color: #f9f9f9;">
  <h1 style="text-align: center;">ICC Men's T20-Cricket World Cup 2022 Data Analytics</h1>
  <p><img src="https://github.com/AnshulChauhan19/World-T20-Team11-/blob/main/JOIN.jpg" alt="Placeholder Image">
  </p>
  <ul>



## Contents:
* ### [Project Overview](https://github.com/AnshulChauhan19/World-T20-Team11-/wiki/_new#project-overview)
* ### [Data Source](https://github.com/AnshulChauhan19/World-T20-Team11-/wiki/_new#data-source)
* ### [Data Gathering](https://github.com/AnshulChauhan19/World-T20-Team11-/wiki/_new#data-gathering)
* ### [Data Processing](https://github.com/AnshulChauhan19/World-T20-Team11-/wiki/_new#data-processing)
* ### [Data Modeling](https://github.com/AnshulChauhan19/World-T20-Team11-/wiki/_new#data-modeling)
* ### [DAX Expressions](https://github.com/AnshulChauhan19/World-T20-Team11-/wiki/_new#dax-expressions)
* ### [Visual Report](https://github.com/AnshulChauhan19/World-T20-Team11-/wiki/_new#visual-report)
* ### [Tools and Libraries](https://github.com/AnshulChauhan19/World-T20-Team11-/wiki/_new#tools-and-libraries)
* ### [References](https://github.com/AnshulChauhan19/World-T20-Team11-/wiki/_new#references)




## Project Overview:
This project involves creating a Power BI Dashboard to review and compare the performances of all players in the ICC Men's T20 Cricket World Cup 2022. The dashboard also helps in selecting the best XI players of the tournament based on predefined criteria included in the problem statement.



## Data Source:
The data was collected from [ESPN Cricinfo](https://www.espncricinfo.com/) and player career performance data was gathered from [Bright Data](https://brightdata.com/).



## Data Gathering:
Data scraping techniques were used to collect match data and player performance data from ESPN Cricinfo. The collected data includes various statistics and metrics relevant to the tournament.



## Data Processing:
The raw data was cleaned and transformed using Python and Pandas. This process included removing duplicates, handling missing values, and converting data types.



## Data Modeling:
The transformed data was then modeled to create relationships between different datasets. This modeling was done using Power BI to enable detailed analysis and reporting.



## DAX Expressions:
Data Analysis Expressions (DAX) were utilized to create calculated columns and measures to enhance the data analysis capabilities within Power BI.

Some of the Measures used in visualization are:

* Total Runs = SUM(t20_batting_summary[runs])

* Total Innings Batted =COUNT(t20_batting_summary[matchID])

* Total Innings Dismissed = SUM(t20_batting_summary[Out])

* Batting Avg = DIVIDE([Total Runs],[Total Innings Dismissed],0)

* Total balls faced =SUM(t20_batting_summary[balls])

* Strike rate = DIVIDE([Total Runs],[total balls faced],0)*100

* Batting Possition = ROUNDUP(AVERAGE(t20_batting_summary[battingPos]),0)

* Boundary % = DIVIDE(SUM(t20_batting_summary[Boundary runs]),[Total Runs],0)*100

* Avg. balls faced =  AVERAGE(t20_batting_summary[balls])

* wickets = SUM(t20_bowling_summary[wickets])

* Balls Bowled = SUM(t20_bowling_summary[balls])

* Runs Conced = SUM(t20_bowling_summary[runs])

* Economy = DIVIDE([Runs Conced],([Balls Bowled]/6),0)

* Bowling Strike Rate =DIVIDE([Balls Bowled],[wickets],0)

* Bowling Avrage = DIVIDE([Runs Conced],[wickets],0)


## Visual Report:
The visual analysis was performed using Microsoft Power BI Desktop, creating various reports to highlight player performances.

## Player Analysis
## Openers:
<p><img src="https://github.com/AnshulChauhan19/World-T20-Team11-/blob/main/Openers.PNG" alt="Placeholder Image">
  </p>

## Middle Order:
<p><img src="https://github.com/AnshulChauhan19/World-T20-Team11-/blob/main/Mid%20Order.PNG" alt="Placeholder Image">
  </p>

## Finishers:
<p><img src="https://github.com/AnshulChauhan19/World-T20-Team11-/blob/main/Finisher.PNG" alt="Placeholder Image">
  </p>

## All Rounders:
<p><img src="https://github.com/AnshulChauhan19/World-T20-Team11-/blob/main/All%20Rounder.PNG" alt="Placeholder Image">
  </p>

## Bowlers:
<p><img src="https://github.com/AnshulChauhan19/World-T20-Team11-/blob/main/Fast%20Bowler.PNG" alt="Placeholder Image">
  </p>

## Best XI Players:
<p><img src="https://github.com/AnshulChauhan19/World-T20-Team11-/blob/main/Team%2011.PNG" alt="Placeholder Image">
  </p>






## Tools and Libraries:
*  Jupyter Notebook
*  Python
*  Pandas
*  Web Scraping
*  Beautiful Soup
*  Power Query Editor
*  Power BI
*  Anaconda Environment


## References:
* [Codebasics Courses](https://github.com/AnshulChauhan19/World-T20-Team11-/wiki/_new#references)
* [ICC Men's T20 World Cup 2022 Official Site](https://www.espncricinfo.com/series/icc-men-s-t20-world-cup-2022-23-1298134/namibia-vs-sri-lanka-1st-match-first-round-group-a-1298135/full-scorecard))
* [ESPN Cricinfo Match Results](https://www.espncricinfo.com/records/tournament/team-match-results/icc-men-s-t20-world-cup-2022-23-14450))
* [ESPN Cricinfo Scorecard](https://github.com/AnshulChauhan19/World-T20-Team11-/wiki/_new#references)
* [Bright Data Collector](https://github.com/AnshulChauhan19/World-T20-Team11-/wiki/_new#references)


  </ul>
  </div>
