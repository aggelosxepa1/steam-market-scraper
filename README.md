# Steam Market Scraper

A script for scraping the Steam Community Market for CS2 items based on a price range you choose.

**Features:**
- Proxy rotation and async proxy validation
- Selenium-based dynamic content handling
- Skips unwanted item types (keys, cases, stickers, capsules,
  package, music kits and patches)
- Saves results to Excel with clickable item URLs
- Handles multiple pages automatically

**Environment**
- Python 3.10.0

**Library Versions:**
- aiohttp: 3.12.15
- beautifulsoup4: 4.13.4
- selenium: 4.34.2
- webdriver-manager: 4.0.2
- urllib3: 1.26.20
- pandas: 2.3.1
- openpyxl: 3.1.5

**Note:**  
The `proxies.txt` file contains free proxies. Free proxies can be slow, unreliable, or may stop working at any time.\n 
For more stable performance, consider using paid or private proxies.
