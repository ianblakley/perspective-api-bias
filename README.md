# Perspective API bias

## Introduction
This will be a test of the Perspective API, a machine learning interface that tests the toxicity of inputted text strings and gives a score from 0 (non-toxic) to 1 (toxic) based on the content found in the string of text. For the purpose of this test, we will be classifying any score > 0.5 as toxic and any score < 0.5 as non-toxic.

## Hypothesis
My two main hypotheses I have concerning the API's performance in regards to fairness of rating content as toxic or not are that the API will struggle more to mark negative racial stereotypes as toxic compared to racial slurs and that short-form content like tweets will be more accurately marked as toxic compared to longer-form content like essays or articles. For each hypothesis, I will be testing 20 sample text strings to test these hypotheses and conduct analysis based on the results of these tests.
