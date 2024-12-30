# Starbucks Capstone Challenge

This repository contains the code and analysis of the Starbucks Capstone Challenge, focusing on answering the following questions:
**Which offer is the most successful?**
**The most effective delivery channels for each offer type**
**The predict effective offer model**

The detail analysis can be view on github (jupyter) or via blogspot
https://cuongkin.blogspot.com/2024/12/analyzing-starbucks-promotion-effective.html


**Data Sets:**
The data is contained in three files:

portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
profile.json - demographic data for each customer
transcript.json - records for transactions, offers received, offers viewed, and offers completed
Here is the schema and explanation of each variable in the files:

portfolio.json

id (string) - offer id
offer_type (string) - type of offer ie BOGO, discount, informational
difficulty (int) - minimum required spend to complete an offer
reward (int) - reward given for completing an offer
duration (int) - time for offer to be open, in days
channels (list of strings)
profile.json

age (int) - age of the customer
became_member_on (int) - date when customer created an app account
gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
id (str) - customer id
income (float) - customer's income
transcript.json

event (str) - record description (ie transaction, offer received, offer viewed, etc.)
person (str) - customer id
time (int) - time in hours since start of test. The data begins at time t=0
value - (dict of strings) - either an offer id or transaction amount depending on the record

**Methodology:**

1. **Exploratory Data Analysis (EDA):**
    * Read the data schema to understand the data format.
	* Check for sample value, null, size of data for better understanding data, state
    * Visualizations to understand dataset (how many data, how many column, sample data, etc.).
    * Build the datamart which contains needed information for further analysis
	
2. **Statistical Analysis:**

**Tools:**

* **Programming Language:** Python
* **Libraries:** pandas, numpy, matplotlib

**Repository Structure:**

* **data/:** Stores the raw datasets.
* **notebooks/:** Contains Jupyter Notebooks with the analysis code and visualizations.
* **README.md:** This file.

**Getting Started:**

1. **Clone the repository:** 
   ```bash
   git clone https://github.com/cuongvt/predict-effective-offer/tree/main
