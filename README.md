# Glassdoor Review Scraper WIP

## How to Use
Designed to be agnostic of which company you are scraping all you need to do is the following:

 1. Ensure this code is loaded in a local IDE (Built and tested in VSCode), cloud based IDE's like Google Collab won't work due the requirement for an installed Chrome instance
 2. Ensure you have chrome installed on your device
 3. Run the following blocks of code
 4. When prompted copy in the url to the reviews page of the company who's reviews you want to scrape

	> Example url: https://www.glassdoor.co.uk/Reviews/eBay-Reviews-E7853.htm
	
 5. Entering a glassdoor username and password is optional however the tool will only be able to return the first page of reviews without them, to mitigate risk they are only held in memory long enough to pass to Glassdoor
 6. How many pages of reviews you wish to return, each page holds roughly 10 reviews

## Current Issues

 - Can't be run in headless mode due to the Captcha solving method, currently exploring alternative methods to get around this requirement
 - No unit tests, these will be included before final submission I've just not had time to include them before the formative!
 - Occasionally when signing in it will click the forgot password link instead of the sign in button causing the code to fail, currently looking into a solution
 - No logic to check you're asking for more pages than there are pages for that company, the issue is there's no clear identifier for the page count as they all use the same class and identifiers. solvable problem just not have time to implement before formative
 - Code is an uncommented mess and needs serious clean up and commenting before final submission