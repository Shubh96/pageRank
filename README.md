# pageRank
pageRank is a *Simple Python Search Spider*, *Page Ranker*, and *Visualizer*. This is a set of programs that emulate some functions of a search engine.  They store their data in a **SQLITE3** database named 'spider.sqlite'.  This file can be removed at any time to restart the process. 
The goal is to provide a simple implementation of [Google's Page Rank](https://en.wikipedia.org/wiki/PageRank) algorithm used in its search engine to rank various search results in order. Google's search engine is way more complex and advanced than mine, but the base implementation remains the same. Google crawls through the entire World Wide Web and gets all links before applying its page ranking algorithm, which needs a very high performing computing system and huge storage. In my implementation, we start with a single URL, crawl through it and identify the ranks of various links that originate from this URL. 

I will provide the implementation details of the algorithm along with an explanation of what the code does. I shall soon upload a complete video showing the implementation of the project on YouTube; but as of now, I leave the read me with only the implementation details using the code files given.

## Requirements
There are very few requirements to run this code. They are listed below:

 - **BeautifulSoup:**  Make sure, when you run the code, whether with normal installation of Python or through [anaconda environment](https://anaconda.org/anaconda/python), you must have the BeautifulSoup module installed.
You can do that by using the command `pip install bs4` in the prompt/environment.
-**SQLite:** SQLite normally comes in the standard library and hence you don't need to install it separately. But, just in case you need to, then you might want to refer to [this](https://stackoverflow.com/questions/19530974/how-can-i-install-sqlite3-to-python) thread at Stack Overflow.
- **SQLite DB Browser:** If you wish to see your database contents without having to execute SQL scripts every time, you would like to install [SQLite Browser](https://sqlitebrowser.org/) in your system.

In order to see the visualization in the browser, make sure you have a JavaScript enabled web browser. Other than these requirements, there are no other dependencies. 

## Using the code
In the code repository, you will find several Python files. To use the algorithm, see the following steps on how to execute the code.

 1. Execute the script `spider.py`. It will ask you to enter the starting URL and you may give any website link. It will also ask for the number of pages you want to crawl through. To get a good visualization, use at least 100.
 2. You might want to dump the contents of the database file, so execute the script `spdump.py`
 3. Run the page rank algorithm on the crawled pages by executing the `sprank.py` script. It will ask for the number of iterations and you can give any number. Try out yourself and see how different values of iterations change the result.
 4. [Optional] Run the `spdump.py` script to see the changes in page rank.
 5. If you want to visualize the current top pages in terms of page rank,
run `spjson.py` to write the pages out in JSON format.
 6. Run the force.html file to see the visualization on the web browser. This shows an automatic layout of the nodes and links.

## How code works
### spider
[Will be added soon]
### spdump
[Will be added soon]
### sprank
[Will be added soon]
### spjson
[Will be added soon]
### force.html
[Will be added soon]
