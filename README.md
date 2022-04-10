# bank-campaign-pyspark-machine-learning
Bank campaign analysis using machine learning with pyspark

[//]: # (<img src="https://user-images.githubusercontent.com/69020265/162612014-ce0e196c-cd5c-4ef3-a311-68698bdd7652.png" alt="drawing" width="200"/>)
<img src="https://user-images.githubusercontent.com/69020265/162612163-f839c2a1-bdd6-410b-8126-731236b08e86.png" alt="drawing" width="200"/>



# Data Set

https://archive.ics.uci.edu/ml/datasets/Bank+Marketing

## Bank Marketing Data Set 

Abstract: The data is related with direct marketing campaigns (phone calls) of a Portuguese banking institution. The classification goal is to predict if the client will subscribe a term deposit (variable y).

<ul>
<li>Data Set Characteristics: Multivariate</li>
<li>Number of Instances: 45211</li>
<li>Area: Business</li>
<li>Attribute Characteristics: Real</li>
<li>Number of Attributes: 17</li>
<li>Date Donated: 2012-02-14</li>
<li>Associated Tasks: Classification</li>
<li>Missing Values? N/A</li>
</ul>

## Source:

[Moro et al., 2014] S. Moro, P. Cortez and P. Rita. A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems, Elsevier, 62:22-31, June 2014


## Data Set Information:

The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed. 

There are four datasets: 
<ol>
<li>bank-additional-full.csv with all examples (41188) and 20 inputs, ordered by date (from May 2008 to November 2010), very close to the data analyzed in [Moro et al., 2014]</li>
<li>bank-additional.csv with 10% of the examples (4119), randomly selected from 1), and 20 inputs.</li>
<li>bank-full.csv with all examples and 17 inputs, ordered by date (older version of this dataset with less inputs).</li>
<li>bank.csv with 10% of the examples and 17 inputs, randomly selected from 3 (older version of this dataset with less inputs)</li>
</ol>
The smallest datasets are provided to test more computationally demanding machine learning algorithms (e.g., SVM). <br>

The classification goal is to predict if the client will subscribe (yes/no) a term deposit (variable y).<br>


## Attribute Information:

<b>Input variables:</b><br>
<br>
<b>bank client data:</b>

<ol>
<li>age (numeric)</li>
<li>job : type of job (categorical: 'admin.' ,'bluecollar' ,'entrepreneur' ,'housemaid' ,'management' ,'retired', 'self-employed', 'services', 'student', 'technician', 'unemployed', 'unknown')</li>
<li>marital : marital status (categorical: 'divorced', 'married', 'single', 'unknown'; note: 'divorced' means divorced or widowed)</li>
<li>education (categorical: 'basic.4y', 'basic.6y', 'basic.9y', 'high.school', 'illiterate', 'professional.course', 'university.degree', 'unknown')</li>
<li>default: has credit in default? (categorical: 'no', 'yes', 'unknown')</li>
<li>housing: has housing loan? (categorical: 'no', 'yes', 'unknown')</li>
<li>loan: has personal loan? (categorical: 'no', 'yes', 'unknown')</li>
<br>
  <b>related with the last contact of the current campaign:</b>
<br>
<br>
<li>contact: contact communication type (categorical: 'cellular', 'telephone') </li>
<li>month: last contact month of year (categorical: 'jan', 'feb', 'mar', ..., 'nov', 'dec')</li>
<li>day_of_week: last contact day of the week (categorical: 'mon', 'tue', 'wed', 'thu', 'fri')</li>
<li>duration: last contact duration, in seconds (numeric). Important note: this attribute highly affects the output target (e.g., if duration=0 then y='no'). Yet, the duration is not known before a call is performed. Also, after the end of the call y is obviously known. Thus, this input should only be included for benchmark purposes and should be discarded if the intention is to have a realistic predictive model.</li>
<br>
<b>other attributes:</b>
<br>
<br>
<li>campaign: number of contacts performed during this campaign and for this client (numeric, includes last contact)</li>
<li>pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)</li>
<li>previous: number of contacts performed before this campaign and for this client (numeric)</li>
<li>poutcome: outcome of the previous marketing campaign (categorical: 'failure', 'nonexistent',  'success')</li>
<b>social and economic context attributes</b>
<li>emp.var.rate: employment variation rate - quarterly indicator (numeric)</li>
<li>cons.price.idx: consumer price index - monthly indicator (numeric) </li>
<li>cons.conf.idx: consumer confidence index - monthly indicator (numeric)</li> 
<li>euribor3m: euribor 3 month rate - daily indicator (numeric)</li>
<li>nr.employed: number of employees - quarterly indicator (numeric)</li>
<br>
<b>Output variable (desired target):<b>
<br>
<br>
<li>y - has the client subscribed a term deposit? (binary: 'yes', 'no')</li>
</ol>

## Relevant Papers:

S. Moro, P. Cortez and P. Rita. A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems, Elsevier, 62:22-31, June 2014

S. Moro, R. Laureano and P. Cortez. Using Data Mining for Bank Direct Marketing: An Application of the CRISP-DM Methodology. In P. Novais et al. (Eds.), Proceedings of the European Simulation and Modelling Conference - ESM'2011, pp. 117-121, Guimaraes, Portugal, October, 2011. EUROSIS. [bank.zip]



## Citation Request:

This dataset is public available for research. The details are described in [Moro et al., 2014]. 
Please include this citation if you plan to use this database: 

[Moro et al., 2014] S. Moro, P. Cortez and P. Rita. A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems, Elsevier, 62:22-31, June 2014

Make analysis without duration
  
Confusin matrix

