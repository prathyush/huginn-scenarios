# huginn-scenarios
Huginn scenarios for specific workflows I use.

### BookMyShow now showing.

This scenario helps keep track of any new English movies in town (India only) which has a decent Metacritic score. Does the following:
  * Scrapes the data off BookMyShow city URL. Set to 'bengalure' by default.
  * Filters out based on language. Set to 'English' by default.
  * Scrapes Metacritic for the score
  * Filters based on minimum score.
  * Post to Slack through a web hook to a desired channel.

### Metacritic reviews.

This scenario will feed you with any interesting movies being rated in Metacritic.
  * Listens on Metacritic Movies RSS feed.
  * For a new item, scrapes the data off the movie page and gets the score.
  * Filters based on minimum score.
  * Post to Slack through a web hook to a desired channel
