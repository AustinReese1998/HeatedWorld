# [HeatedWorld](https://www.heated.world) - [www.heated.world](https://www.heated.world)

- Designed by Ahmad Osman and Austin Reese

- Fetching news from Reddit; /r/worldnews
  - [Reddit API](https://www.reddit.com/dev/api/)
    - [PRAW](https://github.com/praw-dev/praw) - [Documentation](https://praw.readthedocs.io/en/latest/)
  - Top 40 articles in the last 24 hours
  - Top 120 articles in the last 7 days
    - Arranged based on number of votes...
- Parse articles text content
  - [Newspaper3k: Documentation](https://newspaper.readthedocs.io/en/latest/) - [GitHub](https://github.com/codelucas/newspaper)
- Extracting geographical info
  - [Mordecai](https://github.com/openeventdata/mordecai)
    - [Mordecai requires Geonames gazetteer running in Elasticsearch, all through Docker](https://github.com/openeventdata/mordecai#installation-and-requirements).
- Creating world heatmap
  - [Datamaps](http://datamaps.github.io/)
  - Heatmap depends on Reddit's post date(on scale of 1-7) + the number of votes; formula = 1-(n/7). Past 24 hours news should create the initial heatmap first based on votes, and from their a ratio can be taken for the amount of heat the older news will get.
- Potential ideas
  - Creating submaps for each country, with headlines and links to articles and reddit discusions
  - Tags' maps, not just location maps. Doesn't have to be a heatmap though.
  - We can have seperate maps for the last 24 hours and the whole week.
  - List for our calculated scores, last 24 hours, and last 7 days headlines
- Digital Ocean
  - Python3 and Docker...
