# MiLB Stats Dashboard
_Building a data pipeline for MiLB analysis_

## History
As an avid fantasy baseball player, I'm always looking for a way to get an edge on my opponents. As an avid data professional, I'm always looking for ways to hone my skills. Enter this project.

I'm deep enough in the fantasy baseball world to be in leagues that roster 1000+ players, so it takes some digging to identify talent. Ultimately, the goal of this project is simple: build an automated dashboard for personal use that pulls in data points that I value when looking for productive baseball players.

## Methodology
- I wrote and tested the Python code in Jupyter Notebooks. The function loops through 8 Fangraphs API URLs using Request + BeautifulSoup to get the relevant MiLB data, writes the JSON to a Pandas dataframe, and loads that data into a Google Sheet.

- I was able to automate this code using Pipedream's free account (you can use up to 10 credits daily). Very easy interface to work with!

- The workflow is triggered at 9am daily, the script is run, and then it refreshes the dataset for my Power BI dashboard.

- Once the flow has run, it sends me an email to let me know.

Ultimately, this was just a fun little project for me and my niche baseball nerdiness. So far, I've used the dashboard to identify some under the radar up and coming stars so I can add them in various fantasy baseball leagues.

 You can find the Power BI report [here](https://app.powerbi.com/view?r=eyJrIjoiMDg0YmExOTEtNzNlYS00NGQxLTg4NTUtZGVmODU3MTRmNjY2IiwidCI6IjEwMWRhNTg3LTE4NDMtNGY1Mi04YjhhLTE3YjA2OWM2NmQzMyIsImMiOjJ9). Don't judge me - I'm a Tableau guy! I'm looking forward to using this project to flesh out my Power BI skills. 

## Future Research
- Spin up a Postgres or Snowflake server and store historical data for point in time and rolling trends.
- Build out ML model to try and predict future success with past results.
