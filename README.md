# weka-iris
this is the first project on weka workbench its a multiclassification problem on iris dataset
# data observation
iris is a small dataset of 150 instance(3 classes balanced)
it has 4 input attribute about same range (0-8)
there is no missing values

Looking across the graphs for the input variables, we can see good separation between the
classes on the scatter plots. For example, petalwidth versus sepallength and petalwidth versus
sepalwidth are good examples. This suggest that linear methods and maybe decision trees and
instance-based methods may do well on this problem. It also suggest that we probably do not
need to spend too much time tuning or using advanced modeling techniques and ensembles. It
may be a straightforward modeling problem.

# experiment
in  this part we will experiment the 8 following algorithms to see what fit this problem
– rules.ZeroR
– bayes.NaiveBayes
– functions.Logistic
– functions.SMO
– lazy.IBk
– rules.PART
– trees.REPTree
– trees.J48

note: some algorithms have diferent names in weka like 
smo-->support vector machine
ibk-->knn
and so on

#result in accuracy
Dataset (1) rules.Ze | (2) bayes (3) funct (4) funct (5) lazy. (6) trees (7) trees
--------------------------------------------------------------------------------------------
iris (50)     33.33  | 95.47 v      96.33 v   96.33 v  95.20 v   94.27 v  94.53 v

# reference
book: machine learning mastery with weka chapter 2


the result show that logistic regression and smo do the same on this problem so we choose the logistic because it is much simpler

# model
the model is writen in binary formate so to run it we need weka 3-8-6
