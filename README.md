# data-analysis-projects-with-python
This project is built to keep track of my practices in data analysis. I am particularly interested in machine learning and NLP, so the tasks I focus on will be prediction, recommender system and so on. For each project, I usually learn and duplicate others' works first, and figure out what methods they were using and what functions they were creating. One thing I try to improve is that I tend to adopt the lazy way and adjust some of the coding. For example, instead of specifying the column names manually and putting them in the coding, I would rather make computer identify the right ones. And therefore, when dealing with another dataset with similar task, I can apply and revise the script with much less effort.

Another thing is that I like to explore approaches. Usually when I find a brand-new problem, I often switch to doing research related to this problem. For instance, in the project with Give Me Some Credit, new things I encountered were binning, weight of evidence, and information value. From there, I went on studying optimal binning, chi-square binning, and DecisionTree binning. This is probably because I am a guy of divergent thinking.

There are two main categories of content to be included. First one is the project I practiced. I will show how I processed the data all the way along and present possible barriers. That to say, when I followed the steps in other's scripts, why would this problem happen and cause the script stop running. I will try to explain why it does not work in my trial and demonstrate my work in solving the problem. Second, as I have mentioned, I like exploring new methods, so how I get to understand those new methods will be included. 

The first project I worked on was from Give Me Some Credit, one of kaggle Featured Prediction Competition. It's main goal is to predict the probability that somebody will experience financial distress in the next two years. I acquired many new techniques. For instance, I filled missing values with the method of random forest. Also, I used to detect outliers with Z-score method, but it did not work well in this project. Possilbe reason I was guessing was that the data wasn't normally distributed, so the three-standard-deviation approaches deleted much more observations than I expected. I ended up box-plotting the variables one by one to detect anomalies. I admit I did not like this process for it was so trivious. 

One major technique I would emphasize is using information value to select features. information value of each variable represents their predictive power in the model. The calculation of information value is based on data discretization. The method I used in this project was decision tree binning. The principle behind it is entropy. Other discretization approaches I learned were optimal binning and chi-square binning. Speaking of binning, one important method used in Python is pandas.cut(). I reviewed it a little bit.

The purpose of binning was to calculate the weight of evidence and therefore information value. As I said, information value is for feature selection, and for tasks like evaluating credit card score, weight of evidence transformation is quite a common practice. It is said that after weight of evidence transformation, the probability of defaulting and WOE values of variable tend to be monotonic, positive or negative, depending on the nature of the variable.

As for feature selection, I went on studying other approaches such as recursive feature elimination.

Last but not least, there was a severe skew in the class distribution. One approach to addressing the problem of class imbalance is to randomly resample the training dataset. The two main approaches to randomly resampling an imbalanced dataset are to delete examples from the majority class, called undersampling, and to duplicate examples from the minority class, called oversampling. In this case, I used undersampling.

Basically, above is a brief picture of how I will present my work. I am not going to include every project here.

Last, I am doing this to enhance my own learning, not to teach. If I want to present it, I got to organize the content as well as my language. I've never done this, but it is good to try. And you are very welcomed to point out my mistakes. I will be really grateful.
