This project combines four datasets to attempt to predict NHL prospect career success in the form of flurry-adjusted expected goals.
Five North American amateur leagues were analyzed for the prospects they produced, based on number of players drafted from these leagues:
- OHL (Ontario Hockey League)
- QMJHL (Quebec Major Junior Hockey League)
- WHL (Western Hockey League) -- includes mostly western Canada, but some United States Pacific Northwest teams
- ECHL (East Coast Hockey League) -- United States East Coast; but has expanded to include more teams across the United States
- USNDTP -- United States National Development Team Program

Flurry-adjusted expected goals are a statistic calculated by multiplying the probability of a shot on goal scoring by each shot.  So, the more high-quality shots a player
takes, the higher their expected goals statistic will be.  "Flurry adjustment" simply means adjusting expected goals so that when there is a "flurry" of shots (a lot of shots
on goal in a very short period of time), expected goals is not overinflated.  The formula for flurry adjusted expected goals is: chance of not scoring in a flurry yet * regular
expected goal value of a shot.
Data was compiled from four sources:
 - NHL.com (prospect rankings)
 - Hockey Reference (Actual Player Selection Order)
 - Elite Prospects (amateur statistics for prospects)
 - MoneyPuck (containing career flurry adjusted expected goals).
Six machine learning models were utilized to attempt prediction.  Three were types of linear regression:
- LASSO
- Ridge
- Mixed (50-50 LASSO/Ridge)

Three were types of decision trees:
- Bagged Foresting
- Random Forest
- Boosted Trees

Results were mixed, with none of the models performing extremely well.  But bagged and random foresting were the most successful overall in estimating actual flurry adjusted
career goals. This analysis could be expanded to account for more player attributes, such as skating speed and number of hits, and could also be made more nuanced to model
for just one season or league.  It could also be expanded to predict career flurry adjusted expected goals for players from Europe and around the globe, rather than just
North America.
