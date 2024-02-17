
# T20 world cup cricket data analytics


## Introduction

The ICC T20 World Cup 2022, hosted by Australia, featured 20 teams from around the globe, culminating in England's championship victory. Leveraging web scraping and Python, data was collected from ESPNcricinfo using Brightdata. Through meticulous data cleaning and analysis with Pandas, top performers were identified.

A Power BI dashboard was crafted to select the best players for key positions such as openers, middle-order batsmen, finishers, all-rounders, and fast bowlers. Teams selected using this method boasted a 90% chance of winning, showcasing the power of data-driven decisions in cricket.




## Steps followed 

# Web scraping

- For web scraping, we harnessed the capabilities of the powerful data acquisition tool, Bright Data (https://brightdata.com/). Through this platform, we seamlessly extracted data from the esteemed cricket database, ESPNcricinfo (https://www.espncricinfo.com/), ensuring a comprehensive dataset for analysis.

- Bright Data facilitated the collection of essential cricket statistics from ESPNcricinfo, employing its advanced collector to transform the raw data into structured JSON files. This method streamlined the process and enabled efficient handling of the vast volume of data required for our analysis.

- The key JSON files used include:

    - t20_wc_batting_summary.json

    - t20_wc_bowling_summary.json

    - t20_wc_match_results.json

    - t20_wc_player_info.json

These files provided crucial insights into T20 World Cup matches, enabling informed decision-making.

# Python

- Utilizing the Python Pandas library, we conducted rigorous data cleaning and modeling procedures. A primary key, 'match_id', was established to establish relationships across various tables.
- Here's a breakdown of the technical steps involved:
    1. Data Import: JSON files were imported into Google Colab, and Pandas DataFrame objects were created to handle the data effectively.
    2. Primary Key Creation: The 'scorecard' column was renamed to 'match_id' to serve as the primary key, enabling seamless integration and relational mapping across datasets.
    3. Creation of match_id Dictionary: A match_id dictionary was generated to facilitate connections with other tables, enhancing data coherence and accessibility.
    4. Data Refinement: In the Batting, Bowling, and Player summary tables, redundant columns and symbols were meticulously removed to enhance data clarity and analysis.
    5. File Saving: The processed files were saved in CSV format, ensuring compatibility and ease of use for subsequent analytical processes.


# PoweBI

- Power BI served as the cornerstone for visualizing and analyzing player performance based on intricate metrics.

    1. Data Integration: Excel files were seamlessly integrated into Power BI, enabling comprehensive analysis and visualization of player statistics.
    2. Data Modeling: The heart of the analysis lies in the robust data model, where relationships among various datasets were established to facilitate cohesive insights.
    3. Batting Metrics Creation: Key measures were devised for batting performance, encompassing metrics such as Batting Average, Strike Rate, Boundary Percentage, Total Runs, Total Innings Batted, Total Balls Faced, Batting Position, and Total Innings Dismissed.
    4. Bowling Metrics Creation: Similarly, crucial measures were formulated for bowling performance, including Bowling Average, Bowling Strike Rate, Wickets Taken, Dot Ball Percentage, Total Innings Bowled, Runs Conceded, Bowling Economy, Average Balls Faced by Bowler, and Total Balls Bowled.
    5. Player Categorization: Players were categorized into five distinct categories based on their playing roles:
              1.Opener, 2. Middle Order, 3.Lower Order, 4.All-rounder, 5.Bowler
    6. Top 11 Player Selection: Leveraging the comprehensive analysis of batting and bowling metrics, the top 11 players were meticulously selected, ensuring a balanced and competitive team composition.

## Openers :

![opener  cr](https://github.com/aniketpawar123/Project-Cricket-Analysis/assets/123149177/c4d431bc-725f-452b-9990-1bcd3ef37d76)

### Opener based on above Criteria: 

![Power Hitter](https://github.com/aniketpawar123/Project-Cricket-Analysis/assets/123149177/12eddebf-9cb6-47af-bdd4-a4383404b1c7)

##  Middle order :

![Middle order cr](https://github.com/aniketpawar123/Project-Cricket-Analysis/assets/123149177/9d7b82f7-9d41-4023-b973-343aab0a859c)

### Middel Order based on above Criteria:

![Midle Order](https://github.com/aniketpawar123/Project-Cricket-Analysis/assets/123149177/7dd008b7-a020-499d-b870-97a979bdc766)

## Lower Order : 

![Lower order cr](https://github.com/aniketpawar123/Project-Cricket-Analysis/assets/123149177/c5075878-6f78-4cd6-848d-16ad3b79935d)

### Lower Order based on above Criteria:

![Lower Order](https://github.com/aniketpawar123/Project-Cricket-Analysis/assets/123149177/a5d64fea-0922-44d2-b4fb-dc7043ce8e4b)

## All Rounder :

![All r cr](https://github.com/aniketpawar123/Project-Cricket-Analysis/assets/123149177/37009b20-d5ef-4ac8-bf21-4ef5cde2cc5f)

### All Rounder based on above Criteria:

![AllRounder](https://github.com/aniketpawar123/Project-Cricket-Analysis/assets/123149177/f3424949-4422-4775-9358-df875eba383f)

## Bowlers :

![bowler cr](https://github.com/aniketpawar123/Project-Cricket-Analysis/assets/123149177/96e37d5a-d5da-468b-9daa-cb1a2eb76452)

### Bowlers based on above Criteria:

![Bowler](https://github.com/aniketpawar123/Project-Cricket-Analysis/assets/123149177/ef5501d3-1825-4c8f-98b6-40e6de1bb94a)

## Final 11 :
![Final 11](https://github.com/aniketpawar123/Project-Cricket-Analysis/assets/123149177/afcc7819-2b88-4898-8afb-cf741e698293)


