# nba-game-predictor-
Building a model that predicts the outcome of basketball games


Sports betting is becoming more popular by the year. Basketball is one of the more difficult sports to bet on, as underdogs beat good teams on a nightly basis. In this python model, the strategy is to use matrix completion techniques to estimate game outcomes. It will compares two different teams going against one another. There will be mutiple statistics that come into play, combineding pace estimations, defensive ratings, vegas odds, and more. Throughout the NBA season the model with get more accurate as more data is accumulated from games.  

To make predictions, use the following code:

>> model = NBAModel(update=True)
>> model.get_scores('PHO', 'WAS')
PHO WAS
92.9092883132 97.1806398788

which predicts the Suns will lose to the Wizards 93-97.
Note, scraping all the data required to run the algorithm is slow. This only needs to be done the first time. On subsequent models, you can use update=False to used the cached data.
