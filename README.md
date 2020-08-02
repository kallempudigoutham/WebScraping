# WebScraping
Crawling and Scraping with WEB SCRAPY

pip install scrapy

# to start project

scrapy startproject project_name



# to crawl a project


scrapy crawl posts
scrapy crawl posts -o posts.json // stores output to json

# getting data from response css selectors

response.css('h3::text').get()
response.css('h3::text')[2].get()
response.css('h3::text').getall()
response.css('title::text').get()

# xpath selectors

response.xpath('//h3')   // returns all h3 tags
response.xpath('//h3/text()').extract() // returns text of all h3 tags
response.xpath('//h3/text()').getall() // returns text of all h3 tags
