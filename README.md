# 2025_NPORS

Read the substack article [here](https://georgesantellano.substack.com/p/trouble-brewing-in-the-2026-midterms).

The objective of this project was originally to understand a data set which I thought was interesting. With politics all over a news, I wondered if I could use this data to predict the polical party of a respondent to this survey using their responses to a variety of opinion/demographic questions. Along the way, we unnearted a few intersting insights from the mind of Americans. 

Each feature name has a description [here](https://github.com/gesantel/2025_NPORS/blob/main/NPORS_2025_codebook_FINAL.xlsx).

[This](https://github.com/gesantel/2025_NPORS/blob/main/2025%20NPORS.ipynb) is the Jupyter notebook for the analysis. 

Tools used: Scikit-learn, matplotlib, seaborn, pandas, numpy. 
Features: Responses to demographic and opinon questions. 

Target variable: Political party. 

## Data Collection
I gathered this data from the [Pew Resource Center Database](https://www.pewresearch.org/tools-and-datasets/). 

## Data Preprocessing
The data came numerically encoded which was nice but that meant I had to map the numbers back to categories for some of the feature analysis. I used a train test split. 

## Model and Fitting

I used 3 skikit-learn classifiers: Radom Forest Classifier, KNeighbors Classifier, and AdaBoost Classifier which I paramter-tunend with GridSearchCV. 
