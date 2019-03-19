# Monte Carlo Simulations for a Kanban/Agile Flow

## WHY - Facts over Opinions
Estimates are based on gut feeling. Gut feeling is subjective and situative. It is intangible and hard to quantify and share. On the other hand, data can be measured, collected, reported, and analyzed — even visualized. It can objectify discussions and enrich decision making through forecasts.

Benefits of forecasting with a monte carlo simulation instead of estimating (in Story Points):
* Save time of scarce ressources (the team): No planning poker.
* More realistic planning: Data basis of the past includes everything (vacations, sick days, outliers, ...)
* The forecast can be discussed and enrich decision making by chosing the risk the team/management wants to take.

Further thoughts on Agile metrics and #NoEstimates (with a focus on how to collect data and use it with a sense of responsibility):
[You must be this tall to use agile metrics](https://medium.com/@jabopiti/you-must-be-this-tall-to-use-agile-metrics-9d2e3b4d4e20)

## HOW - Building a Monte Carlo Simulation Based on Historical Throughput Data
The idea is to use [Monte Carlo Simulation](https://simple.wikipedia.org/wiki/Monte_Carlo_algorithm) based on historical throughput data to determine a probable range of delivery dates or of total items completed.

## WHAT - Using the Simulation Results to Enrich Decision-Making
In this repository are two Jupyter Notebooks. Each of them generates a notebook calculating the throughput and running a monte carlo simulation to determine how many items can be completed in a given time range or when a given scope of items can be completed. The result of a monte carlo simulation is a visualiziation mapping the probability and the outcome.

The notebook represents a decision-making basis to determine the risk a team/management wants to take to achieve a specific outcome. A 70% probability is risky, a 85% probability is moderate, and a 95% probability is the safe option.

The notebooks are filled with an example to get a better idea on how to use them.

Conditions:
* You need a instance of Jupyter Notebook and Python >3.6 to run the notebooks
* The notebooks use data extracted from Jira with [Jira-to-Analytics](https://github.com/ActionableAgile/jira-to-analytics).

### Kanban-Monte_Carlo-How-Many.ipynb
Determine how many items can be completed in a given time range.

### Kanban-Monte_Carlo-When.ipynb
Determine when a given scope of items can be completed.
