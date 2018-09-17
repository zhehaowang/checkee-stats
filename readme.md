# Checkee Stats

US visa administrative processing time data analytics in Python.

* [Data source](checkee.info)
* Retriever - scrapy
* Analyzer (histogram) - numpy and matplotlib

### How to use

Scrape latest checkee.info reports
```
cd src/retriever
scrapy crawl checkee
```
This will populate src/retriever/data folder.

Customize filter criteria (edit analyze.py) and run analyze
```
cd src/analyzer
./analyze.py
```
This will filter from src/retriever/data folder and produce a histogram of the processing time of filtered entries.