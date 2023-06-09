# APAN_5210_Python_Project

## Motivation
You work as a Data Analyst for a company that sells a Point of Sales (POS) system to small to medium businesses in the US. Your company has hundreds of thousands of clients and continues to grow. (Maybe you work for Square, maybe Shopify, maybe Stripe, etc…) One of the sales teams got their hands on a dataset of business names and locations and they were trying to identify the companies that are not on the platform, in other words prospective sales targets. You have been tasked with determining the overlap between the list of prospective businesses and the internal client list.

## Problem Statement
You are given two datasets:
- left_dataset.csv
- right_dataset.csv

These datasets contain business names and their addresses. The goal of this project is to find the businesses that are common to both datasets, that is, the businesses that have a name and address that match between the left and right datasets. These datasets come from different sources and so there may be some subtle differences between records, even if they do refer to the same business.

Since the business names and addresses don't align perfectly between these datasets, you will need to develop an algorithm that can find approximate matches. When your algorithm runs, it should produce a list of triplets consisting of the entity_id from the left dataset, the business_id from the right dataset, and a confidence score. The confidence score should have values between 0 and 1.0 and convey a sense of confidence of the match. An identical match should have a score of 1.0.

Your submission should consist of matches that have a high degree of confidence, e.g. greater than 0.8.

The technical work that you are expected to conduct as part of this project is:
- conduct exploratory data analysis to understand the data, including visualizations
- develop an algorithm that can produces matches across both datasets
- assign a confidence score to your matches

## Summary
After data cleaning, this project used Partial Ratio from FuzzyWuzzy python package. 

FuzzyWuzzy is a popular library to perform string comparison and matching. The partial ratio feature calculates the ratio of the length of the longest common substring to the length of the shorter string. Useful when dealing with data containing typos, misspellings, or some strings only appear in the longer piece of text.

## Uploaded Files
- left_dataset.csv
- right_dataset.csv
- Function.py
- 5210_project_Python_Warrior.ipynb
- Matching_result_Python_Warrior.csv
