# Part 1: understand the problem
## 00. Background
![avatar](https://github.com/Cecilia-xu/DREAM_SUB2/blob/master/background.png)
## 01. Type of the problem
The goal of sub-challenge 2 (SC2) of the DREAM Preterm Birth Prediction Challenge is to determine how accurately the maternal whole blood transcriptome from two or more samples collected during pregnancy (17-36 weeks) in asymptomatic women, can predict preterm birth.
 
To be more specific, this is a classification problem. Participants are required to develop parsimonious models (at most 100 total unique genes can be involved) to make two sets of predictions for all individuals in the test set. The first set of predictions will classify individuals in the test set as sPTD vs Control, while the second prediction will classify individuals as PPROM vs Control.

## 02. Dataset
The training set includes microarray data from 38 women (including Controls, sPTD, or PPROM) as  well as data from 161 patients  (including Controls, sPTD, or PPROM) The training set has therefore data for 2 or more samples from 196 women (435 samples total) while the test set is composed of data from 87 women (304 samples total).

## 03. Metric
- Area under the ROC curve (AUC) statistic 
- Area under the precision recall curve (AUPR) 

These two will be calculated for each of the two classifications tasks (sPTD and Control, and PPROM vs Control) on the test set, using only data from patients that are actually part of the groups involved in each of the two classification tasks. 
