# JobHunter

The challenge here was to scrape job listing results from several oil company career sites, then amalgamate the results into a single, searchable DataFrame. Scraping data from dynamic web pages is, it seems, no easy task and the code is difficult to maintain. But it's been a good learning experience.

New to web scraping, I quickly realised these sites are difficult to scrape as the search results are paginated (spread across multiple pages), e.g. 25 results at a time. The script must navigate to and iterate over each set of results, appending each to a DataFrame. Also, as the content is dynamic and prone to change, the script is not robust and can easily break. Of course, each site is entirely unique and the format of each job listing can be inconsistent.

The script uses Selenium module to perform webscraping of two sites, Hallibuton and BP career sites, as I found these to be the easier to scrape. It retreives only the job's headline information (role, location, etc.), and not the detailed content behind each listing.
