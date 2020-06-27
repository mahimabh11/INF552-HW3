Readme for Assignment-3

Name: Mahima Bhargava
USC ID: 3936853735

1.The libraries used:

a.) Scikit-Learn
b.) Numpy
c.) Matplotlib
d.) Pandas
e.) Statsmodel
f.) Seaborn
g.) OS
h.) Bootstrapped


Note:
1.) I have handled the missing values in the folder-sitting dataset8, by copying the value of the row above(13250) for the time 13500. This was done using Excel itself.

2.) Bending2-dataset4 was cleaned using python code.

3.) 'trainlist' and 'testlist' are lists of dataframes of train and test instances, respectively. 'train_y' and 'test_y' contain the folder-name, i.e, the actual class of each of the train and test observations, respectively.

4.) F1-score has also been included in some places as a comparison metrics. In classification, it acts as a better scoring method than accuracy as it considers both precision and recall.

5.) In case I am getting multiple options for l-p pairs with the same accuracy(=1), I am opting for the l-value which is the lowest.

6.) I have used reference code to calculate the p-values for the coefficients in 1(d)iv. The link for the code is

    https://gist.github.com/rspeare/77061e6e317896be29c6de9a85db301d

7.) For question 1(d)vii, I have upsampled the samples and have maintained the 4:1 ratio with majority:minority to ensure we do not increase the variance of parameter estimates too much. 

8.) For 1(f), I have used cv=3 instead of cv=5 as bending2 has only 4 observations and to maintain stratified-fold, I reduced the number of folds to 3. 

9.) For question 1(f)ii, I experimented with GridSearchCV and found that the results for multinomial with a given range of alpha values, gives the the same l-value as cross_val_score() function. For Gaussian, I had not entered any parameters and it gave the same result as cross_val_score(). I chose to simply use cross_val_score() and commented the code for GridSearchCV.


