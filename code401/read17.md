# Web Scraping

Web Scraping is a technique to automatically access and extract large amounts of information from a website.

Notes about web scraping:

1. Read through the websites terms and conditions to understand how to legally use the data.
2. Make sure you dont download data at too rapid a rate because it will cause the website to break

**Inspecting the website**

- The first thing you need to do is figure out where to locate the links to the files that you want to download
- You will search through the websites code and find the html tags that correlate to what you're looking to find

**Python code**

Import the following

```
import requests
import urllib.request
import time
from bs4 import BeautifulSoup
```

Then set url to the website and use requests library

```
url = 'http://web.mta.info/developers/turnstile.html'
response = requests.get(url)
```

- If the access was successful you should get a 200 error code

Next, parse the html with BeautifulSoup

```
soup = BeautifulSoup(response.text, “html.parser”)
```

Then use the ".findAll" method to locate html tags

```
soup.findAll('a')
```

**Steps to take to ensure you don't get blocked**

1. Respect the Robots.txt file
2. Make the crawler slower so that you don't harm the server
3. Don't follow the same crawling pattern
4. Make requests using proxies, and rotate them
5. Rotate user agents and HTTP request headers between requests
6. Use a headless browser
7. Beware of honeypot traps
8. Check if the website is changing layouts
9. Avoid scraping behind a login
10. Use captcha solving services