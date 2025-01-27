# DALICodeSample

CNNHTML is a folder containing all of the HTML from CNN that I manually had to download. This file contains article links from a search page present on CNN filtered for only politics articles.
cnn_large_cleaned.txt is the resulting scraped HTML. Each webpage is accessed and the HTML is downloaded, it is then cleaned to only contain the actual paragraphs of information from the articles.

In scraping_cnn
process_html_file - this function is how a file in CNNHTML is processed. The information is cleaned up and then returned. At this point it is still essentially only a bunch of links
In the following section of code, every single file in CNNHTML is iterated through and processed to select only the article URLs.
The next code is used to save the resulting file of exclusively all the article urls
The next code which starts with "Step 2: Define the file path," this code changes the article urls to be a list without any whitespace, then every single URL is looped through and the contents of the paragraphs are saved to a new file so it can be used to train the model.
