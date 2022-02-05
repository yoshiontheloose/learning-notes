# Web Scraping

## Web Scrape with Python in 4 minutes

[Source](https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460)

**Web Scraping** - A time saving technique where you can automatically access and extract large amount of information from a website

Always read the site's terms and conditions for legal use of their data. Using the data for commercial purpose is prohibited on most sites.

Rapidly downloading data could break the website. If this happens, you may be banned/blocked from the site.

### Inspecting the Website

`Inspect` the HTML tags for file links you want to download

`<a>` tag is used for hyperlinks

Import the following libraries:

```markdown
import requests
import urllib.request
import time
from bs4 import BeautifulSoup
```

url is set to the site  
site is accessed with the requests library

```markdown
url = 'http://bigolwebsitename/something.html'
response = requests.get(url)
```

Successful access will have an output of a `response 200`

BeautifulSoup is used to parse the html to provide a more readable and nested data structure

```markdown
soup = BeautifulSoup(response.text, "html.parser")
```

To locate all `<a>` tags, use .findAll() method

```markdown
soup.findAll('a')
```

Grabbing one `<a>` tag

```markdown
one_a_tag = soup.findAll('a')[line number of desired link]
link = one_a_tag['href']
```

Click the data file on the website to get the file path.  
To download that file path, we use `urllib.request` library.  
`request.urlretrieve` will need two parameters: file url and the filename.

```markdown
download_url = 'http://some.sitename.info/something/'+ link
urllib.request.urlretrieve(download_url, './'+link[link.find(/something_')+1:])
```

Pause the code from running with this function to avoid getting flagged due to spamming the site with requests

```markdown
time.sleep(1)
```

## What is Web Scraping?

[Source](https://en.wikipedia.org/wiki/Web_scraping)


## How to scrape websites without getting blocked

[Source](https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/)

---

# Videos

## Track Amazon Prices

[Source](https://www.youtube.com/watch?v=Bg9r_yLk7VY)

---

# Bookmark/Skim

## Beautiful Soup

[Source](https://www.crummy.com/software/BeautifulSoup/)

[<<<Back](README.md)