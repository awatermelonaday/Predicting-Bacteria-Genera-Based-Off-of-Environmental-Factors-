# Predicting-Bacteria-Genera-Based-Off-of-Environmental-Factors-
## Project Description
This project will result in an app that will allow people to enter in sampled environmental factors to calculate what possible generas there could be in the sample. The purpose of this project is to simplify the prediction process of these bacteria taxas. Tools and websites used include Google Colab for data cleansing and the machine learning program, and Thunkable for creating an app. We are using a public data set from Dryad called “Saw Kill river (NY, USA) metagenomics and environmental variables” for building a prototype program. 

## First Day of a New Project 11/21/26 (awatermelonaday)
- Today I worked on creating the repository for Predicting Bacteria Genera Based Off of Environmental Factors
- I found two useful public datasets from DYRAD and sent them over to Vivian
- The main problem with this data set was that it included over 3000 different bacteria generas, however most of this data was just 0 and we believed this was not of any use to us for the moment (as for now we are just trying to make a prototype)
-  Vivian started and made great progress on the Data cleaning process to the point where it was almost done
### Next Steps: 
- Finish the data cleaning process
- combine taxonomical data set with the environmental factor data set

## Data Combination 11/22/26 (awatermelonaday)
- Today I worked on preparing the bacterial abundance (taxanomical) and environmental datasets for the actual machine learning part of this project (though I have not gotten there yet)
- aligned environmental variables with the corresponding bacterial samples to prep for combining the two data sets
- DID end up combining the two data sets!
- (But) before I did that I looked at what columns had a bunch of missing values, to which I decided that those columns may mess up the predictions when we actually get to training a machine learning model, so I ended up dropping columns that contained 50 or more missing values. (This really just meant I dropped a bunch of columns with 70 ish missing values as all the other columns only had 0-4 missing values)
- I also dropped the Dates column because I did not think it contributed to our project as all the dates were the same
### Next Steps
- update the combined dataset by renaming all the columns into just the names of the genera instead of the full taxonomical classification for the sake of simplicity
- split environmental predictors into (X) and bacterial genera abundance data into (Y)
- Begin training Random Forest model 
