# Solana Sniper Bot

This Solana Sniper Bot snipes new token pairs based on customizable filters. The bot allows you to automate the buying process of new tokens on the Solana blockchain with specific conditions to avoid rug pulls and other risks.

Snipe all fresh new pairs in two clicks.



https://github.com/bigmovers/solana-sniper-bot/assets/165174061/06287e80-08aa-43b3-90f0-2443ccb36a7d




**TELEGRAM** for contact & **POC**(Proof of Concept) & **VOUCHES**: [@benorizz0](https://t.me/benorizz0)

Support in running the tool is included in the price.

Watch out for other scammers on GitHub - they either sell my outdated code which doesn't work anymore or simply selling blank files.

**Other tools**
- [Volume Maker JITO/Non-JITO](https://github.com/bigmovers/solana-volume-bot)
- [Solana JITO Bundler](https://github.com/bigmovers/solana-bundle)
- [Pump.Fun Bundler(25buys)](https://github.com/bigmovers/pumpfun-bundler)
- [Buy/Holder Maker](https://github.com/bigmovers/solana-maker)
- LP Manager
- Telegram Cloner


## Features

- Customizable buy amount and tip amount
- Minimum SOL requirement check before trading
- Retry mechanism for failed transactions
- Rug pull protection filters
- Snipe list with filter and refresh interval
- Telegram integration for automated trading via a bot

## Configuration

Update the configuration settings in the script to customize the bot behavior:

### Buy Settings

```ini
BUY_AMOUNT_SOL=0.02 # Amount of token to buy in SOL
JITO_TIP_AMOUNT=0.005 # Amount of token to tip to Jito
MIN_SOL_REQUIRED=0.1 # Minimum amount of SOL in your wallet required to trade
MAX_BUY_RETRIES=2 # Maximum retries to buy a token if txn failed
BUY_DELAY=0 # Delay in milliseconds before buying token
```

### Rug Check Filters
```ini
MIN_SOL_LP=4  # Minimum SOL used to create a liquidity pool
MAX_SOL_LP=20 # Maximum SOL used to create a liquidity pool
MIN_TOKEN_LP_PERCENTAGE=70 # Minimum percentage of token supply in liquidity pool
MAX_TOP10_HOLDERS_PERCENTAGE=40 # Maximum percentage of token owned by top 10 holders excluding Raydium
MAX_SINGLE_OWNER_PERCENTAGE=13 # Maximum percentage of token owned by a single holder
```

### Rug Check Toggles
```ini
ENABLE_RUG_CHECKS=true # Enable all rug checks toggled with true
CHECK_MINTABLE_AND_FREEZABLE=true # Check if token is mintable and freezable
CHECK_TOP10_HOLDERS_PERCENTAGE=true # Checks holders percentage
CHECK_BURN=false # Checks if LP is burned
CHECK_IF_SOCIALS=true # Checks if token has socials added
TOKEN_SYMBOL_FILTER="BONK" # Token symbol to filter snipe list
CHECK_TOKEN_SYMBOL=false
```

### Telegram integration and auto-sell strategy using Trading Bot like [trojanbot](https://t.me/hector_trojanbot?start=r-benorizz0)
```ini
TG_API_ID=
TG_API_HASH=
TG_SESSION_ID=
TG_BOT_USERNAME='@hector_trojanbot' # Change to the username of the TG bot you are already logged in with
```




