This project uses a logistic regression model to attempt to predict cardiovascular disease based on a variety of parameters. In it we will build four different models and determine which one is the best one based on AUC and accuracy. After we find which model is the best, we will then determine how good it is by looking at various scores. These scores will hopefully allow us to make valuable insights about our models usability. 

Necessary Packages: 

import pandas as pd
import numpy as np
import sklearn
from sklearn import linear_model
import sklearn.metrics as metrics
from sklearn.metrics import accuracy_score
import matplotlib.pyplot as plt
import random

Code can simply be ran through and will depict scores at the end with conclusions documented as well.



Conclusions: Our final graph shows our ROC curve and shows the balance between sensitivity and specificity. Our precision is our ability to predict our positive outcomes correctly and our recall is our ability to predict our negative outcomes correctly. As we can see, our recall is 1 which means we predict our negative outcomes perfectly. However, our precision is 0.584 which means our positive predictions is only slightly better than random.  This is shown in our ROC curve with our AUC only being 0.68 which is not great as well. When thinking about our data and what we are working with, we are trying to predict cardiovascular disease in patients. We have a 100% chance of telling someone if they do not have cardiovascular disease which is great. However, we only have a 58.4% of correctly predicting when someone has cardiovascular disease. Thus, in my opinion, this is not a very good model and shouldn’t be used to help predict cardiovascular disease. 
