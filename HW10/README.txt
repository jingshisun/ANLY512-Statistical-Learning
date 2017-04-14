Complete these problems in a well-written RMarkdown document and upload the corresponding PDF or html file. 

1. Write up your work of 4/4/17 (15 points)
Write up a report on your groups’s in class work of Tuesday, 4/4. The report should give a short introduction to the specific problem that you looked at, explain data cleaning and data wrangling that may need to be done, give some data exploration (tables, histograms, scatterplots, boxplots, whatever explains the data well), and carry out the computations that are in the problem description for your dataset. Take a look at all the code that was uploaded to the forum on Tuesday, learn from your fellow students’ work and improve on it.

Details are in the Discussion area.

2. A classification problem (10 points)
Consider the R workspace ex0408.RDataView in a new window which is available in the Files area. It contains two dataframes of 10,000 observations each, one for training and one for testing. The goal is to predict  the variable  z  from the other ten variables.

Each observation is a sorted random sample of size 10 from {1, 2,…, 200}. Then z = TRUE if the sample contains two numbers where the smaller one divides the larger one, and z = FALSE otherwise.

Fit a tree to the training data. Evaluate it for the training and the test data, using a confusion matrix. Comment on the performance. This is the baseline case.

Use bagging. Show that it is possible to obtain a perfect fit on the training data. Evaluate the model on the test data. Comment on the performance.

Use a random forest approach. Show that it is possible to obtain a perfect fit on the training data. Evaluate the model on the test data. Comment on the performance.

Use boosted trees to predict z. How well can you fit the training data? How well do these models perform on the test data? For a boosted tree, the variable z should be in {0,1}. Fit a model with a really large  n.trees  value. The predictions will be numbers in the interval [0,1]. You can then predict to 1 if the predicted value is > 0.5 (e.g.) and to  0  otherwise, just as in the case of logistic regression.

