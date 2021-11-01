# Financial Planning with APIs and Simulations

![Photo of notebook with pen and the words Financial Planning](https://lh3.googleusercontent.com/proxy/fUQKeaUwogRPKPMQVPw1Z7-GNPHUxAGkbWqGuyZmFcnJ1qL_7E5_ZDcsE0XgNTnkNxI4_Gd2taXKnQtengkL_t3QLeLD2NiQI8-QmUb4VLY)  

---
This program evaluates a credit union member's current financial holdings using API calls for current prices. It then evaluates if the member has enough holdings to create an emergancy fund (three months income). A Monte Carlo simulation is run to forcast probable financial futures for different portfolio proportions over 10 and 30 years. This is to give the member a range of likely outcomes which they will then use to determine when to retire and how much their savings would likely be worth at such time.

---
## Technologies:

This program runs on [Python 3.7](https://www.python.org/) and utilizes [Jupyter Lab](https://jupyter.org/install)


---
## Installation Guide:

Before you open the program you must obtain both an ALPACA_API_KEY and an ALPACA_SECRET_KEY. To do this, you must have or create an account with [Alpaca Markets](alpaca.markets) and 'Generate' your personal keys.

Open `financial_planning_tools.ipyn` using Jupyter Lab and store both of the keys in a seperate file named `.env` using this syntax:

```python
ALPACA_API_KEY = "put_your_alpaca_api_key_here"

ALPACA_SECRET_KEY = "put_your_alpaca_secret_key_here"
```

Import the following libraries for the program to run:

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

---
## Usage:
Load in the `.env` file you created using ```load_dotenv```.

Once you start moving through the program you will then start seeing outputs that look like this:

![Screen shot of a pie chart](https://user-images.githubusercontent.com/89755088/139623202-21252b65-14f8-4ee0-933d-0dd58407296b.png)

![Screen shot of a graph](https://user-images.githubusercontent.com/89755088/139621787-43c40c42-b6b2-4ed8-b31f-8208fff41b96.png)

---
## Contributors:

Code written for use and functionality was done by Thomas Leahy, thomasleahy6@gmail.com

In conjunction with © 2020 - 2021 Trilogy Education Services, a 2U, Inc. brand.

---
## Licence:

MIT

2021 Thomas Leahy