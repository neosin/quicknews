# QuickNews

A Python/SQLite3 program that web scrapes BI Tech articles, archives them in a NEWS database, and generates cards of bit-sized information.

1. Articles are stored as objects, containing:
    - title: The title of the article
    - bullets: The bullet summaries of the article
    - url: The url of the article for more information
    - date: The published date of the article

2. Beauitful Soup is utilized to scrap news information from websites, particularly identifying:
    - title as h1 tags with class="post-headline"
    - bullets as ul tags with class="summary-list"
    - date as div tags with class="byline-timestamp" and attribute "data-timestamp"

The default url for scraping the Tech section of BI website is: http://www.businessinsider.com/sai

The program runs through the headlines/articles of the Tech page. Each headline/article contains a url to their respective article, from which the title and bullet summaries are extracted. With Bootstrap 4 and Jinja2, the articles are aggregated as cards onto a single viewable page automatically opened. 

Running "python quicknews.py" starts the fun...

"This is a personal project made for fun. All Respective icons and service(s) belong to Respective owners."