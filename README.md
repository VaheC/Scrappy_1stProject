# Scrappy_1stProject

* scrapy startproject "project name here"
* go to spiders directory and scrapy genspider "spider name here" "URL here"
* "shell = ipython" in scrapy.cfg and run "scrapy shell"
* run fetch("https://books.toscrape.com/") to save html content inside scrapy shell
* the outcome of the above step is in response variable, so we can use it to get various parts of the html (example: response.css("article.product_pod") or response.css("article.product_pod").get())
* exit scrapy shell using exit command
* go one level up to bookscraper directory and run "scrapy crawl bookspider" in bash
* run "scrapy crawl bookspider -O bookdata.json" to save data in json (overwrites)
* run "scrapy crawl bookspider -o bookdata.json" to save data in json (appends)
* add FEEDS to settings.py and run "scrapy crawl bookspider" without specifying a file name
