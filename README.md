# Korean Baseball statistics

## Before I started..
Hi this is the final project of Data visualization and I tried make a plot of Korean baseball statistics.

## Data
This is South Korea baseball league plot. It has 5 features (AVG, ERA, RANK, Attendance, Year)

### Year
I used baseball data from 2000 to 2015.

### AVG
AVG means batting average. Normally AVG over 0.3 batter is a great batter. If you want to know about this, please click the [link](https://en.wikipedia.org/wiki/Batting_average).

### ERA
ERA means pitcher Earned run average. run means score. For pitcher, low ERA pitcher is good pitcher.
If you want to know about this, please click the [link](https://en.wikipedia.org/wiki/Earned_run_average).

### RANK
RANK is the rank of korean baseball league. I used regular season rank not post season rank.

### loca1, loca2
location of stadiums

### Attendance
Attendance calculate by team. Korea is so small so It cannot calculated by stadium. when the game opened, one side is for home team and other side (usually 3rd side) is for away team. KBO(Korean Baseball Organization) calculate the attendance using this. If a game (A vs B, A's home) is opened, they calculate each of home and away attendance.

## Chart Explain 1 (map)

### purpose of this chart
see attendance by each region and get some knowledge.

### The bubbles location
locations of stadium.

### The bubbles size
This is the attendance of a team.

### Color of bubbles
Each teams.

## Chart Explain 2 (bubble chart)

### background description of League
ave mean one hit but in baseball there are several hit like single, double, and homerun etc.
so even if the league ave is low that cannot show era is low.
Slugger League : Low avg High era which means batter got more double, homerun than other season.
Pitchers league : Low avg, Low era which means Pitcher dominated the league.
Batters league : High avg, High era which means Batter dominated the league.
Contact league : High avg, Low era which means batter got a lot hit but that couldn't be run


### X, Y axis
they are AVG and ERA. I cut the axis to see more clearly.

### The bubbles size
This is the attendance of a team

### Color of bubbles
This is the rank. First I used several color by each team. However It cannot be readable so I tried to devide 3 group.
Top 2, Bottom 2 and others.

### Right side bar
IT is total yearly attendance of Korean baseball League. and also It can be a console to see the plot yearly.

## Plot and Interpret

### Plot

I used dimple.js specifically, [this example](http://dimplejs.org/advanced_examples_viewer.html?id=advanced_storyboard_control)

This is plot and code

the first plot
http://bl.ocks.org/crespo86/40273e11f516d9c0fbe858193a5550f6#file-index-html

the final plot

http://bl.ocks.org/crespo86/9851e479cf01a70d81255a51dade6f80#file-index-html

### Plot Design

- map + bubbles
  - People want to see the attendance by location and the map is the best way to make it.
  - I used bubbles for attendance because bubbles are really good to compair each location and show pregress by year.

- scatter chart + bubbles
  - I want to show property of league by year using team stats. Using scatter chart, I can see the aggregation of team stats by years. 
  - for the first time, I thought name of tean is not important in this plot because I want to see the aggregation to understand league stuation by year. However some feedback want to see the stats and attendance by team in this graph. so I used team color and attendance as bubbles.

### Interpret

I want to find some relationships with some features and attendance.

1. map
  - Korean baseball League attendance is growing up. (See right bar)
  - Bears, Twins, Giants has large attendance
  - left upper side is Seoul, which is capital of Korea.
  - right down side is Busan, which is second city in Korea.
  - Twins attendance did not change however Giants attendance change alot.
  - Even though total attendance is growing up, Lions, Tigers, Eagles need to struggle more to gather attendance.
  - in 2015, Tigers and Eagles made their new stadium and it might have an effect to grow up their attendance.

2. Stats
  - Korean baseball League attendance is growing up. (See right bar)
  - High Rank team doesn't High attendance. (Blue team is not normally High scale)
  - High **league** AVG make more Attendance than High league ERA. (it can be hard to understand cuz my fool english. In korea, the season which is pitchers dominate league call pitcher's era and the season which is batters dominate league call batter's era. In the plot most of team located at bottom left, it is pitcher's era and if they are located at top right, it call batter's era. in batter's era, usually increased attendance.)
   
## Feedback

1. from Southkorea baseball community mlbpark.com

  - they said.. era and avg is not matched.... they need era and OPS but southkorea baseball data don't have ops cuz we just adpot [sabermatrix](https://en.wikipedia.org/wiki/Sabermetrics).

  - they want to see the attendance in regional data.

  - a guy said when I make map data, I should make bubble by stadium of their team cuz this data need not just team data but region data. for example, unicorns change their stadium alot.

2. from udacity forum

  - a guy said i need to change color looks clear.
  - the guy want to see the Rank

3. what I change and what I didn't change

  - I couldnot find OPS of Southkorea league so I couldn't
  - I made map in stadium data
  - I change bubble color

### reference

1. udacity forum
2. [mlbpark.com](mlbpark.com) (korean baseball community)
3. [statiz](www.statiz.co.kr/) (korean baseball statistic site)
4. [stackoverflow](http://stackoverflow.com/) (d3, dimple usage)
5. [dimplejs](http://dimplejs.org/) (example and API documentation)
6. [d3.js](https://d3js.org/) (example and documentation)
7. [korean map.json](https://github.com/southkorea/southkorea-maps)
8. [google map](https://www.google.co.kr/maps?source=tldsi&hl=ko) (find log, lat)
