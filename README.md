# Twitter-Signal-Cryptocurrency-Buyer

John McAfee has decided to tweet about a coin everyday for 50 days. So far every coin that he was tweeted about has jumped over 100% within the first few minutes of his tweet. This bot is built to take advantage of that.

The bot waits for John to tweet, parses the tweet and uses OCR on any images to get the full text of the tweet and searches for the coin name. It then checks to see if the coin is listed on either Binance or Bittrex. If it is on one of them, the bot uses all the Bitcoin in the account to buy the coin.

# Instructions for use

Go to your Bittrex account, click Settings, API Keys and create a Key with READ INFO, TRADE LIMIT, and TRADE MARKET ON. Make sure that WITHDRAW is OFF.

Create a file in the main folder called bittrex_secrets.json and fill it with your key and secret in the format below.

```
{
  "key": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "secret": "xxxxxxxxxxxxxxxxxxxxxxxxxxxx"
}
```

Go to your Binance account, click account, Api settings and get your API key and secret.

Create a file in the main folder called binance_secrets.json and fill it with your key and secret in the format below.

```
{
  "key": "xxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "secret": "xxxxxxxxxxxxxxxxxxxxxxxx"
}
```

Create a twitter Application here https://apps.twitter.com/app/new and get your consumer_key, consumer_secret, access_token_key, and access_token_secret.

Create a file in the main folder called twitter_secrets.json and fill it with your information in the format below.
```
{
  "consumer_key": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "consumer_secret": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "access_token_key": "xxxxxxxx-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "access_token_secret": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
}
```

Get an API key from https://ocr.space/ocrapi and put it in a file in the main folder called ocr_secret.json in the format below.


```
{
  "api_key": "xxxxxxxxxxxxxxxxxxxx"
}

```
Then just make sure you have Bitcoin in both of your accounts, turn it on at night.
Make sure the seen_coins.txt list is updated before you start or else it might buy a coin that's already been pumped.
