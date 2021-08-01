# *Financial Planning with APIs and Simulations*
---
With Jupyter notebook we will create two tools: a financial planner for emergencies, and a financial planner for retirement.

The financial planner for emergencies will allow users to visualize their current portfolio of both stocks, bonds, and cryptocurrency, and determine if they have enough reserves for an emergency fund.

The financial planner for retirement will forecast the performance of their retirement portfolio in 30 years from now, as well as a 10 year scenario where stocks are more heavily weighted than bonds.  It requires making an Alpaca API call via the Alpaca SDK to get historical price data to use in Monte Carlo simulations.

---
## Technologies:

The Jupyter file utilizes python 3.7 along with the following libraries and dependencies:

os

requests

json

pandas

dotenv

alpaca_trade_api

MCForecastTools

matplotlib

```python
    import os
    import requests
    import json
    import pandas as pd
    from dotenv import load_dotenv
    import alpaca_trade_api as tradeapi
    from MCForecastTools import MCSimulation

    %matplotlib inline
```

Please create your own .env file with your unique Alpaca API Key and Alpaca Secret Key in order for the Alpaca API calls to work.

```python
ALPACA_API_KEY = "<YOUR ALPACA API KEY HERE!>"
ALPACA_SECRET_KEY = "<YOUR ALPACA SECRET KEY HERE!>"
```

---

## Contributors

kevin-mau

---

## License

MIT