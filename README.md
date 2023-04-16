# Data-Science-Tools
A selection of tools which may help speed up manual tasks when collecting, cleaning and analysing data.

##1. Article URL Scraper

- Contains two functions for scraping article text from an article given the url. 
- The first function uses the Wayback Machine Archive to access the article, and is more suited for older articles which may no longer be listed on the website.
- The second function accesses the article directly using the article url, and is more suited for recent articles.

- On a sample of 30,000 article URLS, both functions successfully scrape text for 60% of the articles.
- Using a combination of both functions, article text was scraped successfully in 80% of cases, with at least one of the functions proving effective for each article.
