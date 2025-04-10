# TweetControversyMeter
## Overview
- The goal of this project is to create a tool that can predict the general sentiment of replies to a tweet. Users would input text that they're thinking of posting on Twitter and the tool would predict probabilities to predict if that post would garner positive responses, negative responses, or divided responses from users.  
- Essentially, it would act as a PR tool to vet potential tweets
## General Development Approach
- The plan is to take a tweet API and group a tweet with its replies
- We would then analyze the replies for sentiment, scoring tweets with more interaction higher to create a positive/negative/divided sentiment label
- Then we'd find a model that can predict a reply sentiment score for a tweet
## Considerations/Risks
- Main risk is bias; a tweet that uses words that might not be well received by some users on the app could be well received by its followers. This could cause incorrect predictions
- Finding a suitable model to match a tweet to its response sentiment could be difficult; if we're unable to find a good model then this project would fail
- Another consideration is that a single reply to the original tweet may influence or alter the sentiment of the replies grouped under the original tweet. A reply that disagrees with the original tweet that is followed by several replies concurring with the disagreement could trick the model into thinking that overall sentiment is high
