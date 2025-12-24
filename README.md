# CS2 Steam Market Buy Order Scraper with Proxy Rotation

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Selenium](https://img.shields.io/badge/Selenium-Automation-green)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Processing-blueviolet)
![Proxy Rotation](https://img.shields.io/badge/Proxy-Rotation-orange)
![License](https://img.shields.io/badge/License-MIT-red)

A script for scraping the Steam Community Market for CS2 items based on the item type and price range you choose, filtering items by their latest buy order price instead of listing prices.

**Features:**
- Proxy rotation and async proxy validation
- Selenium-based dynamic content handling
- Skips unwanted item types (keys, cases, stickers, capsules, package, music kits and patches)
- Saves results to a spreadsheet (`steam_market.xlsx`) with clickable item URLs
- Handles multiple pages automatically

## 🛠️ Installation

1. **Prerequisites**
   * Ensure you have **Python 3.10** or higher installed.
   * Make sure **Google Chrome** is installed on your system (required for the automation to work).

2. **Clone the Repository**
   ```bash
   git clone https://github.com/aggelosxepa1/steam-market-scraper.git
   cd steam-market-scraper

3.  **Install Dependencies**
    Install the required Python libraries using the `requirements.txt` file:
    ```bash
    pip install -r requirements.txt
    ```

4.  **Configure Proxies**
    * **Quick Start:** The repository **already includes a `proxies.txt` file** pre-loaded with free public proxies. You can run the script immediately without any setup!
    * **Performance Note:** The included free proxies are often slow or unstable.
    * **For Better Results:** If you have your own **high-quality paid or private proxies**, simply open `proxies.txt`, delete the existing lines, and paste your own IPs (format: `ip:port`).
    
    **Example content for `proxies.txt`:**
    ```text
    192.168.1.1:8080
    203.0.113.5:3128
    198.51.100.2:8000
    ```
    
## 🚀 Usage

Run the script and follow the on-screen prompts:

```bash
python steam_scraper.py
```
    
**Environment:**
- Python 3.10.0

**Library Versions:**
- aiohttp: 3.12.15
- beautifulsoup4: 4.13.4
- selenium: 4.34.2
- webdriver-manager: 4.0.2
- urllib3: 1.26.20
- pandas: 2.3.1
- openpyxl: 3.1.5

## ⚠️ Disclaimer & Risk Warning

**Use this script at your own risk.**

* **Rate Limiting:** Steam strictly limits the number of requests you can make to the Community Market. Even with proxy rotation, excessive scraping can lead to a **temporary IP ban** (HTTP 429) lasting from a few hours to a day.
* **Free Proxies:** The `proxies.txt` file uses public/free proxies. These are often slow, unreliable, or already blacklisted by Steam. For consistent results, usage of high-quality private residential proxies is recommended.
* **Account Safety:** While this script scrapes public data, aggressive automation can theoretically flag your account. It is recommended to use this tool without logging in or with an alt account if possible.
