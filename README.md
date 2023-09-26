# Ethics-Projects

Load the data (application_train.csv – the only file we will use) and provide a basicEDA (Exploratory Data Analysis)
#1 Focus on variables that you consider prone to ethical discussions: what are they?
Highlight and discuss them
#2 Take a look at the training set: are the interesting variables at #1 related to the
target variable? According to their type (binary, continuous, etc.) provide a numerical
and/or visual representation
Hint: For instance, take a look at the gender variable. Do males and females have the
same insolvency ratio, on average? And what about age?
Split the dataset in train and test (80%-20%) and then train a simple ML model (youcan just use the provided code). Evaluate the importance of the different features on
the model
#3 Are the features you found in #1 considered relevant by the trained ML model?
Yes, no, or better: how much?
Hint: Using the provided model, you can start from the standard built-in feature
importance(1). A fancier (and extremely effective) alternative is using SHAP(2) values.
Let’s take a look at the performance of the model on the test set
#4 Ignore the original test target and just take the predictions of the ML model (seeprovided code). Overall, how do the variables at #1 relate to these predictions? Is it
similar to what you saw on #2 and how do you explain it?
Hint: You can exactly rerun the code used on #2. In #2, you analysed some original
train features vs. original train target, on #4 you are analysing test features and test
predictions provided by the ML model
Just take some records from the test set (let’s say 2 or 3) and look at the predictions
of each one
#5 Try and manually alter the sensitive variables (those at #1) and score the new,
altered records: do the predictions change?
#6 You’ve analysed the overall behaviour of your ML model on the test set (#4) and
even double checked on some individual cases (#5): what’s your conclusion? Did the
model learn the differences and biases in the original dataset?
Let’s just remove all the variables of some ethical concerns
#7 Retrain the ML model, score the test set and perform the analysis (#3). What’s the
new AUC performance (with respect to the original one)?
#8 Analyse both the overall behaviour and individual one (#4 to #6). What’s goingon? Do we still see differences for the average predicition of different groups?
Hint: Should we consider gender, remove the variable but keep track if a record
belongs to one group or another (M or F)! This way you can analyse if removing the
variable is enough or somehow the differences in the average predictions remain…
Time to wrap up
#9 Did results at #8 surprise you? Can you explain why just removing the variables
wasn’t enough?
#10 (difficult) Any ideas on different ways to reduce the bias in this specific
problems? What are the difficulties and the tradeoffs we could encounter?

#1 to #6 Understand the data and the business problem we’re facing: what concernsyou from an ethical viewpoint? See how a simple (but not trivial) ML model learns the
characteristics and the biases in a real-world case – MANDATORY
#7 to #9 Try the simplest way to address your concerns, aiming at a bias-less ML
model. Did you solve all the problems? How about the tradeoffs? – OPTIONAL
#10 Are there other alternatives to deal with biases in your dataset? (i.e. what AI
fairness solutions are all about) – OPTIONAL (and quite difficult!)
