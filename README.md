# Perspective API bias

## Introduction
This will be a test of the Perspective API, a machine learning interface that tests the toxicity of inputted text strings and gives a score from 0 (non-toxic) to 1 (toxic) based on the content found in the string of text. For the purpose of this test, we will be classifying any score greater than 0.5 as toxic and any score less than 0.5 as non-toxic.

## Hypothesis
My hypothesis is that the API will struggle to differentiate between text that is quoting/reporting on speech the API determines is toxic and actual speech the API determines as toxic. For example, I believe the API will not be able to consistently identify the difference between a CNN tweet/article reporting on toxic speech versus the actual speech itself. I will take 20 examples of this and determine whether my hypothesis was correct or not.
