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

## Data Refinement + Starting Random Forest Prototype 11/24/26 (awatermelonaday)
- Worked on a new notebook that is just dedicated to making this first prototype *uploaded to this repository as well*
- only started with the basics like importing Pandas, NumPy, and sklearn
- More importantly though for the original clean data program and the combined dataset, I renamed all the columns to actually make since and be readable to be only the genus name
- Yet then, now that it’s neater, I realized that some columns were actually just the same genus again so I just combined those said columns together (which lowered the today columns which is sad because that’s less data than I thought we had to work with)
- Then what happened was that I realized some of the samples were from water and some were from soil/outflow but I think for this prototype I only want it to be from the actual freshwater river which brought the whole thing down to only 37 rows
- So, TLDR, our sample size is going to be extremely small but I guess that’s ok.. (maybe?) since this is just a first try prototype, I can figure out how to get a bigger dataset later after I have made since of the program, right now I think it will do
- Now back to the random forest model, I started splitting the columns into X and Y variables, like I mentioned earlier the X variables would be the environmental factors with the Y variables being the taxa abundance
- Finally, I checked for missing values again, last time I only filtered out all the columns with large amounts of missing variables so there was still some columns left with missing variables
- I figured out how to solve this though, and I learned something new today, median imputation is when you can use the medican across the column to help repair a missing value. I don’t think this will change results too much because I only had 3 columns with missing values and they each were only missing one value. (But I don’t know, hoping I did the right thing.)
### Next Steps
- fully train the Random Forest model and tweak it until I understand what changing the hyperparameters actually does
- Use it to generate some bacterial abundance predictions (and change parameters to alter the accuracy)
### Overall Challenge
- my biggest challenge today was trying to fix the data cleaning program to make sure the columns and the combined dataset overall was fully prepped and ready to go to start the prototype.
- Now that I am done with this data prepping step I am glad I went through with it as now I have to find a bigger dataset and I will have more experience with it now so it should be more efficient the second time around for the actual model (as again this is still just a prototype)

## Dataset Searching 11/26/26
- Happy Thanksgiving!
- I spent some time today looking for a bigger dataset that consists of only water samples and that of a large amount of samples to train a second prototype/model with
- Didn’t end up finding one that I could actually download (I revisited an old one that would have been great data but my computer kept freezing every time I tried downloading it so I won’t fight it for now and move onto something else that I can actually open)
- The hunt will continue tomorrow, for now that’s all
### Next Steps
- find a downloadable dataset, only water samples, atleast 150+ for a second prototype (hopefully 500+ or 1000+ for the final model), clean that data, and make the second prototype 


