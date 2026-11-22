
The dataset that we chose ultimately is: https://www.kaggle.com/datasets/danielgrijalvas/movies/data

What is our definiiton of a successful movie? 
- iMDb user rating (What would the threshold be for a rating that is considered "successful"?) --> 6/10 will be the cutoff
- If the revenue was at least 2x the budget (justify why we chose to do revenue/budget ratio)
-


Computational Methods:

- Mutliple Regression (assuming a linear relationship) 
- Logistic Regression (do a separate analysis of each feature, compare and graph the output of the regression to see which features have the most measurable impact on the success variable)
- Limitations: mention that the gold standard for this modeling would be XGBoost/random forest
- PCA maybe - output is not very interpretable and not feasible


What are some features of the dataset that might be significant?
- Actor/actress starring in the movie 
- Company that produced the movie
- Runtime 
- Rating
- Genre 
- IMDb score (this one is complicated because it's both a predictor and a measurement of success; if we investigate this one we need to add a note to the graph) 

Which columns are we NOT going to use as defining features?
- Budget (purchasing power difference) - unless we do US only
- Director, actors, writers of the film
- name of the film

Data processing and investigation
- US only (70% of the total dataset anyways, eliminates certain economic covariation)
- Make an initial correlation matrix to preview what relationships might be significant, and based on that, pick which relationships might be worthwhile investigating
- Drop the columns with the missing values - cuts out 29% of our data but it's okay- still 5000 points

Limitations
- We have no idea why those specific movies were chosen to be included in the dataset - potential bias?
- Very few movies rated G - this causes a bias in the distribution of data and prevents us from making a conclusion about G rated movies

WHAT WE NEED TO ACCOMPLISH BY NEXT WEEK:
- Avneet: make a google slides presentation and share it with the rest of the group, take the lead on formatting/preparing slides
- Avneet:  Data processing (US only, drop the missing values)
- Amrita:  Initial correlation matrix
- Nolan: Modify the dataset to add a "Success" column (0 or 1, based on the 2x rule)
- Amrita/Nolan: split up the computational methods stuff - decide how we're going to go about doing them

OUR NEXT MEETING:
- Sunday night - 10 PM over Zoom just to confirm everyone's progress/run through slides
