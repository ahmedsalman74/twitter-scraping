

# Twitter Stock Mentions Scraper

This Python script scrapes specified Twitter accounts for mentions of stock symbols and provides the count of mentions within a given time interval.

## Features

- Scrapes Twitter accounts for mentions of stock symbols.
- Allows specifying the Twitter accounts to scrape.
- Supports specifying the stock symbol (ticker) to search for.
- Allows setting the time interval for scraping sessions.

## Installation

1. Clone this repository:

   ```
   git clone https://github.com/yourusername/twitter-stock-mentions-scraper.git
   ```

2. Navigate to the project directory:

   ```
   cd twitter-stock-mentions-scraper
   ```

3. Install the required Python packages:

   ```
   pip install -r requirements.txt
   ```

## Usage

1. Modify the `accounts` list in the script to include the Twitter accounts you want to scrape.
2. Set the `ticker` variable to the desired stock symbol you want to monitor.
3. Set the `interval_minutes` variable to the desired time interval for scraping sessions (in minutes).
4. Run the script:

   ```
   python scraper.py
   ```

   This will continuously scrape the specified Twitter accounts at the given interval and print the count of mentions for the specified stock symbol.

## Example

```python
accounts = [
    "https://twitter.com/Mr_Derivatives",
    "https://twitter.com/warrior_0719",
    "https://twitter.com/ChartingProdigy",
    "https://twitter.com/allstarcharts",
    "https://twitter.com/yuriymatso",
    "https://twitter.com/TriggerTrades",
    "https://twitter.com/AdamMancini4",
    "https://twitter.com/CordovaTrades",
    "https://twitter.com/Barchart",
    "https://twitter.com/RoyLMattox"
]

ticker = "$TSLA"  # Change this to the desired ticker
interval_minutes = 15  # Change this to the desired time interval

scrape_twitter_accounts(accounts, ticker, interval_minutes)
```

## Dependencies

- requests
- re (regular expressions)
- time

## Notes

- This script may be subject to rate limiting or other restrictions imposed by Twitter. Use responsibly and considerate of Twitter's terms of service.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

You can further customize this README file by adding information specific to your project or providing more detailed usage instructions. Additionally, you may want to include information about contributing, troubleshooting, or any other relevant details for users.