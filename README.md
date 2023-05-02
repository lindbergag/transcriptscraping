# Transcript Scraping
# Web scraping to collect a corpus of Podcast transcripts.

This is a collection of simple python scripts that gathers the text transcript of podcasts from the host website. Given the nature of web-scraping, each script is bespoke, and details for that podcast's script are included in the folder with the project.

## Requirements
* Python 3.6+
* Requests
* BeautifulSoup
* Pandas

## Setup
1. Clone the repository
2. Install the required packages
3. Run the script

## Contributing

Feel free to fork the repository and submit pull requests with any improvements or bug fixes.

## Author's notes

This script will not plug and play into another podcast because most webpages use different structure, formatting, or code. If you want to use this as a framework for something else, consider the following:
* Is there another way I could get this data?
    * Many people are honored to support students. A quick e-mail asking for the information might be a lot faster and easier than writing a script. It also might help you develop a relationship with the team behind the show and who knows where that might take you!
* Does the website allow scraping?
* Does the website use html or javascript (or something else)? 
    * You may not be able to retrieve the information or you may need different packages.
* How is the information displayed on the website?
    * For example: How to Be Awesome at Your Job offers the transcripts for each episode on the pages that contain the links to several episodes. Getting the full text transcript for each episode could have been done without visiting the page for the individual episode. 
        * I could have eliminated the steps where I generated a list of links and the step where I visited the page for each episode. Instead of a 3 second delay between 1,008 page visits (~51 minutes of time), this would have been a 3 second delay between 174 page visits (~9 minutes). 
        * However, after many attempts, I couldn't find a way to gather the title and the publish date for each episode from the pages that contain a list of episodes.
* What do you need to change about how I approached this to get the information you're trying to gather?
* Could you do this in a way that is better optimized?
