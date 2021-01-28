# SEO Notes

## Sources 
- [Moz Beginners SEO Guide](https://moz.com/beginners-guide-to-seo)

## [SEO Intro](https://moz.com/beginners-guide-to-seo/why-search-engine-marketing-is-necessary)
  - If the business operates locally out of a store-front or offers some other face-to-face service, using Google My Business listing is a good tool. 
  - Fulfilling user intent is important, use keyword searching to see the current SERP for the desired keywords.
  - Know the website's goals for SEO and the business goals to focus on a certian aspect of SEO, where to track conversions, and how to set benchmarks. 
    - What are the Key Performance Indicators (KPIS)? Some common KPIs:
      - Sales
      - Downloads
      - Email Signups
      - Contact Form Submissions
      - Phone Calls
    - If the business is using Google My Business, some KPIs for that could be:
      - Clicks-to-call
      - Clicks-to-website
      - Clicks-for-driving-directions
    - More traffic and high ranks are not KPIs, they are a means to an end. Put simply, what's the point of having traffic if they aren't accomplishing a business objective?

## [Crawling, Indexing, and Ranking](https://moz.com/beginners-guide-to-seo/how-search-engines-operate)
  ### Crawling: 
  Scour the internet for content and observe the code/content for URL found.

  - To check how many pages are indexed, search `site:yourdomain.com`. Google will then return all results it has indexed for the site specified.
  - To more accurately monitor results, you can use the Google Search Console. 
  - If the site is not responding with search results, there are some reasons as why that could be:
    - The site is brand new and hasn't been crawled yet
    - The site isn't linked to from external sites
    - The site's navigation makes it hard for the robot to crawl effectively
    - The site contains code called crawler directives that is blocking search engines
    - The site has been penalized by Google for spammy tactics
  - #### Robots.txt
    - Located in the root directory of the website. Used for suggesting what parts of the site should and should not be crawled, and the speed at which they crawl the site by using robots.txt directives. 
      - Can block crawlers from accessing pages like old URLs with thin content, duplicate URLs (ex. sort-and-filter params for e-comm sites), special promo code pages, staging or test pages
    - How Googlebot treats robots.txt
      - If Googlebot can't find a robots.txt file, it proceeds to crawl the site
      - If Googlebot does find a robots.txt file, it will usually follow the directives and proceed to crawl the site
      - If Googlebot encounters an error while trying to access the robots.txt file and it can't determine if it exists or not, it will not crawl the site
    - Optimize for crawl budget
      - Crawl budget is the average number of URLs Googlebot will crawl before leaving a site, so crawl budget ensures that Googlebot doesn't waste time crawling meaningless pages while ignoring important pages. Crawl budget is really important on very large sites with thousands of URLs, but small sites can benefit from configuring the crawl budget as well. Be sure not to block crawlers access to pages that have other directives, such as cononical or noindex tags. If Googlebot is blocked from a page, it acts as if that page doesn't exist and it won't see the instructions on that page. 
    - Be careful handling private content in robots.txt, as malicious bots can use robots.txt to find where sensitive content is placed on the site. It's better to `noindex` those pages and gate them behind a login form rather than place them in the robots.txt file. 
  - #### Defining URL parameters in Google Search Console
    - Google usually does a good job a serving the representative URL on its own, but using the URL Parameters feature in Google Search Console can tell Google exactly how to treat the pages when URL parameters are applied. It can be used to tell Googlebot to "crawl no URLS with ___ parameter", hiding the content from Googlebot, removing those pages from search results. That is good if those parameters create duplicate pages, but not ideal if those pages are supposed to be indexed. 
  - #### Now we know how crawlers work and how to keep them away from the bad content, but are they able to find the *good* content?
    - Is the content hidden behind login forms? Crawlers can't log into a site to view pages
    - Does the site rely on a search form? Crawlers cannot use them
    - Is text hidden within non-text content (like images, videos, GIFs, etc)? If text needs to be indexed, do not put it in non-text content, put it as an actual text element because crawlers do not know how to read images for text very well. 
    - Can search engines follow the site navigation? If a page has to be reached by a means other than following a path of links from the site navigation, a crawler will not be able to find it so it might as well not exist.
    - Common nav mistakes that keep crawlers from working:
      - Mobile nav that shows different results than desktop nav
      - Any type of navigation that are not in the HTML, just as JS enabled navigations. Google can *kind of* crawl JS, but it's still not great. 
      - Personalization, or showing unique navigation to specific types of users vs others, could appear to be cloaking to a search engine crawler 
      -  Forgetting to link to a primary page on the website through navigation - Links are the paths crawlers follow to new pages! 
    - Is there a clean information architecuture? Information architecture is the practice of organizing and labeling content on a website to improve usability and findability for users. An information architecture should be inuitive, users shouldn't have to think hard to use the site or find something.
    - Are sitemaps being utilized? A sitemap is a list of URLs on the site that crawlers can use to discover and index content. One of the easiest ways of doing this is to create a file that meets Googles standards and submitting it to Google Search Console. This will help crawlers, but does *not* replace good navigation! 
      - Be sure to only give URLs that are supposed to be indexed, and give the crawlers consistent directions. Don't put a URL in the sitemap that is blocked by robots.txt, or include URLs in the sitemap that are dupilcates rather than the preferred, canonical version. 
    - Are crawlers experiencing errors when trying to access URLs? View "Crawl Errors" on Google Search Console to detect URLs that are being problematic for crawlers. 
      - 4xx Error Codes - Search engine crawlers can't access the content due to a client error
        - The URL contains bad syntax or cannot be fulfilled. Most common 4xx error is the 404
      - 5xx Error Codes - Search engine crawlers can't access the contnent due to a server error
        - There is a tab in the "Crawl Error" section of Google Search Console dedicated to these errors. This means something went wrong with server when trying to access the page, most typically the URL timed out and Googlebot abandoned the request. 
        - If applicable, investigate the 301 permanent redirect 

  ### Indexing: 
  Store and organize the content found during the crawling process. Once a page is indexed, it has a possibility of being displayed as a search result to a query. 

 
  ### Ranking: 
  Provide pieces of content that will best fulfill a search query, ordered from most to least relevant. 
  

## On-Site SEO
  - META Tags
  - Incoming Links
  - Various On-page Linking Factors

## Link Building

## Technical SEO
  - Technical
  - Canonical
  - Server
  - On-page Indexing

## Keyword Analysis

## Content Checking 

## Site Review
  - Average Site Visits
  - Bounce Rate
  - Site Speed
