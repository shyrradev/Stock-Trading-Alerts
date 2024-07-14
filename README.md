# Stock-Trading-Alerts
# Stock News Alert System

This project is a Stock News Alert System that fetches stock price data and news articles related to a specific company. If the stock price changes significantly, the system sends alerts via SMS using Twilio.

## Features

- Fetches daily stock price data from Alpha Vantage API.
- Checks for significant changes in stock prices.
- Fetches the latest news articles related to the company using the News API.
- Sends SMS alerts with the news articles using Twilio.

## Requirements

- Python 3.x
- `requests` library
- `twilio` library

## Setup

1. Clone this repository or download the script.
2. Install the required libraries:
    ```sh
    pip install requests twilio
    ```
3. Replace the placeholder values in the script (`stock_news.py`) with your actual API keys and phone numbers:
    - `STOCK_API_KEY`: Your API key from [Alpha Vantage](https://www.alphavantage.co/support/#api-key).
    - `NEWS_API_KEY`: Your API key from [News API](https://newsapi.org/register).
    - `TWILIO_SID` and `TWILIO_AUTH_TOKEN`: Your Twilio account SID and Auth Token from [Twilio Console](https://www.twilio.com/console).
    - `VIRTUAL_TWILIO_NUMBER`: Your Twilio virtual phone number.
    - `VERIFIED_NUMBER`: Your own phone number verified with Twilio.

## Usage

1. Save the script as `stock_news.py`.
2. Run the script:
    ```sh
    python stock_news.py
    ```

## Example

Here's an example of the script's output:

```sh
735.11
720.85
1.97
Get News
[{'source': {'id': 'techcrunch', 'name': 'TechCrunch'}, 'author': 'Author Name', 'title': 'Tesla stocks soar...', 'description': 'Description of the article...', 'url': 'https://techcrunch.com/example', 'urlToImage': 'https://techcrunch.com/example.jpg', 'publishedAt': '2021-01-01T00:00:00Z', 'content': 'Full article content...'}, ...]
