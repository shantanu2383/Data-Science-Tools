# Data-Science-Tools
A selection of tools which may help speed up manual tasks when collecting, cleaning and analysing data.

##1. Article URL Scraper

- Contains two functions for scraping article text from an article given the url. 
- The first function uses the Wayback Machine Archive to access the article, and is more suited for older articles which may no longer be listed on the website.
- The second function accesses the article directly using the article url, and is more suited for recent articles.

- On a sample of 30,000 article URLS, both functions successfully scrape text for 60% of the articles.
- Using a combination of both functions, article text was scraped successfully in 80% of cases, with at least one of the functions proving effective for each article.

##2. Factiva Article Scraper

- Factiva is a news and business information database owned by Dow Jones & Company that provides access to a wide range of global news sources, company and industry data, and market research.
- It is possible to download articles as pdf files using the free version of Factiva.
- This code uses regex to extract the article text, publisher, title and word count from the article pdf, and stores the results in a pandas dataframe.
- This code is therefore useful for students/researchers looking to construct a database of news articles and article text quickly and cheaply, without having to subscribe to a premium news media service.

##3. Google Trends Scraper
- This function creates a dataframe of interest on google for a particular search term.
- Since google trends data is restrictive in that it only displays interest in a specific term, we also create a function which generates related terms based on googles auto suggestions using the googlesearch library.

##4. Get Wikipedia Article Title
-One issue we found when working with data on media coverage on stocks, is that the official stock name listed on the exchange is often different to the colloquial name used to reference the stock in the media. (Apple. INC and Apple, Microsoft Corp and Microsoft etc)
-We found that the wikipedia article title often provides a map between the official stock name and the colloquial name.
-This function therefore takes the official stock name as listed on the exchange, and returns the wikipedia article title.
