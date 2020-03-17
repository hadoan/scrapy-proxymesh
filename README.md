# scrapy-proxymesh - Python3

Proxymesh downloader middleware for Scrapy.


## Usage

- Register free acount from https://www.proxymesh.com/
- Create simple-proxymesh-middleware.py in your root-folder
- Copy python code from scrapy-proxymesh/__init__.py, paste to simple-proxymesh-middleware.py

settings.py:

    DOWNLOADER_MIDDLEWARES = {
        'simple-proxymesh-middleware.SimpleProxymeshMiddleware': 100,
    }
    
    PROXYMESH_URL = 'http://username:password@us-il.proxymesh.com:31280'
    
    # Proxymesh request timeout
    PROXYMESH_TIMEOUT = 60

