## Betfair Automation

This repository establishes an automated process to place bets on Betfair using the Betfair API.

You can create an API Account from instructions here https://betfair-datascientists.github.io/api/apiPythontutorial/.

Once you have created an appkey you can embed the key, your username and password in a .env file in this project directory. An example of how a trade is executed and how we login is found in the trade_execution.py file. All helper functions are found in the Driver folder.  

To get around a "TypeError: Type is not JSON serializable: numpy.float64" caused within the betfairlightweightAPI, I extended the JSONEncoder in the betfairlightweight/endpoints/baseendpoint.py file as per the top answer here https://stackoverflow.com/questions/50916422/python-typeerror-object-of-type-int64-is-not-json-serializable
