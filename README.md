# Fantasy Football Cheatsheet Creator
A value-based cheatsheet creator for fantasy football drafts for leagues of any format.

1. Take input from user based on league settings
    - number of teams in the league
    - roster details
    - ppr rules
    - add details to dictionary for later use
2. Scraping ADP
    - use BeautifulSoup scrape player ADP for league's PPR format from [FantasyPros](https://www.fantasypros.com/)
    - create data frames for each positon, ordered by ADP
3. Find replacement players based on ADP
    - use the user's league details to find the ADP of the replacement player, ready to calculate value
4. Scraping player projections
    - use BeautifulSoup scrape player projections from [FantasyPros](https://www.fantasypros.com/)
    - create a data frame for all positions, ordered by prokected fantasy points
5. Calculate value over replacement and output cheatsheet
    - use replacement player dictionary and projection data frames to calculate each player's value over the replacement
    - create data frame ordered by value over replacement
    - save cheatsheet
