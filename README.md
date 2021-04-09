# Starbucks Capstone Project | Udacity - ML Engineer Nanodegree

## Overview

Starbucks Corporation is an American multinational chain of coffeehouses and roastery reserves headquartered in Seattle, Washington. Nowadays the company has more than 30,000 locations worldwide. In order to - amongst others - increase sales it sends different offers to its customers via their Starbucks App, such as plain advertisment, Buy One Get One Free (BOGO) or discounts on various items.

The motivation for this project it to analyze the differenz offer types and investigate them through an EDA approach as well as a ML model. The goal is to use the reactions of customers towards previous sent offers and anticipate their reaction on potential next offers. 

The approach as well as a detailed summary of all findings can be found [here](https://thomas-r-meissner.medium.com/starbucks-capstone-challenge-d36b361ac333).

## Datasets and Inputs

The data sets are provided by Starbucks and Udacity and mimic customer behavior on the Starbucks rewards mobile app. These data sets are:  
- portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)  
- profile.json - demographic data for each customer  
- transcript.json - records for transactions, offers received, offers viewed, and offers completed  

Here is the schema and explanation of each variable in the files:

**portfolio.json**  
- id (string) - offer id  
- offer_type (string) - type of offer ie BOGO, discount, informational  
- difficulty (int) - minimum required spend to complete an offer  
- reward (int) - reward given for completing an offer  
- duration (int) - time for offer to be open, in days  
- channels (list of strings)  

**profile.json**  
- age (int) - age of the customer  
- became_member_on (int) - date when customer created an app account  
- gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)  
- id (str) - customer id  
- income (float) - customer's income  

**transcript.json**  
- event (str) - record description (ie transaction, offer received, offer viewed, etc.)  
- person (str) - customer id  
- time (int) - time in hours since start of test. The data begins at time t=0  
- value - (dict of strings) - either an offer id or transaction amount depending on the record  

## Files
The following files have been added to this repository:
-   **[Starbucks_Capstone_notebook.ipynb](https://github.com/reachanihere/Starbucks-Capstone/blob/master/Starbucks_Capstone_notebook.ipynb)**: This is the Jupyter Notebook in which I performed all my work.
-   **[data](https://github.com/reachanihere/Starbucks-Capstone/tree/master/data)**: This contains the three JSON files provided by Starbucks / Udacity as noted above.

## Acknowledgements
Special thanks to Starbucks and Udacity for providing the data utilized in this project!
