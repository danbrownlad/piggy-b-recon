# piggy-b-recon
Just a quick advanced and powerful*- all-in-one recon tool I made piggy -backing- some of the most prominent tools for bug bounties for personal experimentation £.

Features of piggy-b-recon are:
Create your own custom wordlists with common words and phrases related (but not limited to): client's assets, given words and information, and data strongly correlating to support and development of infrastructure for specified targets scraped from local assets, forums (if any) and developer updates/messages/structure of website etc. (My tool)

The malleable parameters are as follows (the script itsself has instructions on what to change to optimize quality of words): 
The term(s) inputted relating to what you want the tool to analyze, match, pull and crawl for (it is recursive, as all tools should be),

How far you want the tool to look/crawl for the words i.e limit the number of directories you allow the crawler to try and pull words from before stopping the crawling process and sharpening trends and found words in relation to the given sources/words,

The sources of which the code pulls the related words from. (I added comments to instruct you on where to find these assets to scrape words, but also simoultaneously crawl the page for certain in-text values by referencing it back onto the words it already has, relating to the development and support, looking for similarities between the words recursively adding them to the list (with a /n for every value, seriously people start doing this who has time to pull up vim to fix literal code output when you could just add a simple line of code to prepend this event),

And the amount of words you want the script to output of course...



Output the wordlist ready to be utilized by the piggy's recon stage. Domain enumeration: code is structured for functionality, supply variables to pass as arguments to the corresponding tools (yes just change 2 variable values and my code's structure will work it's magic): domains (variable), and the wordlist (variable). Then outputting, filtering and removing duplicates of scraped and brute-forced domains. At this point, you must look through results and take away the domains with response codes you don't need, remove the response codes and the tool will then probe over HTTP (80) and HTTPS (443) and screenshot each valid web-app.


*-in my opinion anyway
