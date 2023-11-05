# Perspective API Testing

## Introduction
This will be a test of the Perspective API, a machine learning interface that tests the toxicity of inputted text strings and gives a score from 0 (non-toxic) to 1 (toxic) based on the content found in the string of text. For the purpose of this test, we will be classifying any score greater than 0.5 as toxic and any score less than 0.5 as non-toxic.

## Hypothesis
My hypothesis is that the API will struggle to differentiate between text that is quoting/reporting on speech the API determines is toxic and actual speech the API determines is toxic. For example, I believe the API will not be able to consistently identify the difference between a news tweet/article report that contains toxic speech versus someone using toxic speech to be rude or offensive. I will take 10 examples of this and determine whether my hypothesis was correct or not.

## Data Collection
To collect data, I searched the Twitter accounts of three mainstream media news sources, namely CNN (@CNN), Fox News (@FoxNews), and The Washington Post (@washingtonpost). While looking through these accounts, I tried to find tweets containing language/keywords that I thought the API might flag as toxic, and compiled them into a Jupyter Notebook for analysis.

## Result
While testing my hypothesis, I found that none of the tweets were marked by the API as toxic, with none of the tweets even getting a score any higher than 33.9%. This disproves my hypothesis that the API would struggle to identify these news tweets as non-toxic, as it got a perfect 10/10 on my sample.

## Potential Biases
A potential source of bias that I noted were in the scores for two of the tweets, one concerning current Speaker of the House Mike Johnson's past actions against the LGBTQ+ community, and another about Former Israeli Prime Minister Benjamin Netanyahu's pro-war stance against Hamas. The first tweet was rated a miniscule 0.00014 toxicity rating by the API, despite the mention of things like anti-gay conversion therapy and the criminilization of gay sex being directly referenced in the tweet. The second tweet was rated a bit higher, a 0.148, but still very far from toxic, which was surprising to me considering the mention of violence, which is directly alluded to in this tweet, earned much higher scores on some of the other tweets, such as a tweet mentioning a mass shooting getting a 0.25. The reason I believe the scores of these two tweets may suggest a bias in the API's algorithm is because tweets the API analyzed that referenced similar content like prejudice and violence, were deemed much closer to containing toxic speech than these tweets were. There are of course also reasons to believe that this may just be the way the API processes this information, and the scores aren't reflective of any bias since they were all under the threshold of toxic content, so one score being higher than another may not mean much.
