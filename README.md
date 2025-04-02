# kaggle-competitions
Rainfall competition:


UNTITLED-12 is the python script for the rianfall playground competition from kaggle(my first serious competition).
The final score (ROC score) on the private leaderboard is of 0.89882 with a ranking of 449/4381.

.EDA & FEATURE ENIGINEERING:

For the training dataset I used a mix of the dataset provided by the kaggle competition and some tweeking on the original dataset provided by stanford.
I feature engineered some features and copied some from public notebooks that looked promising and from that created a weight dictionary for each feature.

.MODEL STRUCTURE:

For the model, I used OOF technique with 3 different basic models than made an optimizer that associated weights to each model to optimze the overall ensemble.
The OOF technique was a technique introduced by top kaggler in the discussion session and said that this technique coud overfit very easily depending on the weights dictionary, So I set up the weight dictionary with very small weight differences plus without any data leakage which made this model less likely to overfit on the test dataset.

.POTENTIAL IMPROVEMENTS:

There was a possibility to introduce better engineered features that used sin or cos because of the time series resemblance of this dataset.
The use of ANN was also an option that I did not explore and hope to explore in future competitions.

