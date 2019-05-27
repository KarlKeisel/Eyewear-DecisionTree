# Eyewear-DecisionTree
Using scikit learn to build a predictor for my sales geomap project.


Hello all!

For my big business project I wanted to add some sort of machine learning into it, such as a recommender system to help give hints on which patients would be most willing to purchase.
Being my first real scikit project I wanted to keep it simple and just focus on cleaning the data and getting a good accuracy. Since I also made the algorithim that determined when and what a patient bought this project was to follow the motions and get a good handle on the basics.
I ended up going with a decision tree for my choice at the end to help predict the "buying group" the patient was in, and exported it so that on the website I designed it would give the people working at my "office" a good idea on who are the big spenders.

Accuracy is at 95%


Fine details:

My first thought was to start with a recommender system to predict items the patient might wish to purchase, and that quickly was going to get out of hand for my first project.
Then I figured I would run with logistic regression to have a % chance to purchase or a scale of how much money a patient was likely to spend. Without going into far more than the standard plug and play I was getting a horrible 40% accuracy.
Next thought was K Means since I had 5 buying groups and I would have a nice 5 clusters. I found out that standard category data was not liked by K Means without processing it far more than I was willing to do for a starting project.
Finally I tried a decision tree knowing that they helped standardize their own data, and required very little to work especially with sorting into my 5 categories. I went one step further and tried out a random forest, but accuracy on defaults did not improve while the cost did. 

However, this model will do horribly on new patients as they have no purchases which was the bulk of my data in the decision tree. If I really spent some time on original buying algorithm, such as setting weights for addresses or having family members, I bet I could have made a decent prediction on even new patients.
