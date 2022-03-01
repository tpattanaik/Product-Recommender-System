# Product-Recommender-System

# Abstract:
In today's modern epoch of information technology, the idea of efficiently finding one's favourite product in a large dataset of application database, becomes an essential issue to address for the online content providers in order to attract the masses as opposed to their competitors. Recommender systems or recommendation systems, as they are popularly known, are information filtering systems which are usually integrated with several consumer and commercial applications. Such systems act as a bridge between various content facilitators such as social media websites, e-commerce portals, streaming platforms, etc. and the users of these applications, by suggesting them items from the application database which conform to the user preferences and past activities. Such personalized systems play a vital role, especially when the user is unclear of the item to the searched for. These systems are infiltrating every aspect of our lives, in the form of ?Because you watched? header on Netflix, ?People you may know? section on Facebook, ?Customers who bought this also bought' partition on Amazon.

# Problem Statement:
Many online businesses rely on customer
reviews and ratings. Explicit feedback is
especially important in the ecommerce industry
where all customer engagements are impacted
by these ratings. Amazon relies on such rating
data to power its recommendation engine to
provide the best beauty product
recommendations that are personalized and
most relevant to the user.

Build a recommender engine that reviews the
customer ratings and purchase history to
recommend items and improve sales for beauty
products.

# Data Summary:

➢
reviewerID UserId

➢
asin ProductId

➢
reviewer Name User
Name

➢
helpful

➢
review Text

➢
overall Rating

➢
summary

➢
unixReviewTime

➢
review Time

# Recommended Systems:

➢
Sharp system that provides idea about
item to users that might interest them.

➢
Recommendation system is subclass of
information filtering to predict
preferences to the items used by or for
users. It personalize recommendation
and deals with information overload.
These demands throws some
challenges so different approaches like
memory based, model based are used.

# Need of recommendation systems:

Recommender systems help in addressing the information overload problem by retrieving the information desired by the user based on his or similar users preferences and interests.

# Approaches of Recommendation System:

Recommendation system is usually
classified on rating estimation:

➢
Collaborative Filtering system

➢
Content based system

➢
Hybrid based system

# Exploratory Data Analysis:

Feature Name- ProductId

![image](https://user-images.githubusercontent.com/85148563/156231433-5b35194d-d825-4ec2-bbd5-153841386b7a.png)

➢
Plotted graph has only
top 10 products.

➢
The graph is showing
how many times a
particular product has
been sold.

Feature Name- UserId

![image](https://user-images.githubusercontent.com/85148563/156231541-b5c630a6-5090-43bc-aeab-d9573d991bcf.png)

➢
Plotted graph has only
top 10 Users.

➢
The graph is showing
how many times a
particular user has
purchased a products.

From chart it’s clear that-

![image](https://user-images.githubusercontent.com/85148563/156231599-b34427d6-e098-46be-b468-c320d15b4bfc.png)

➢
Most of the product has
given as highest rating.

➢
Very less number of
product has low rating.

Before Log Transformation

![image](https://user-images.githubusercontent.com/85148563/156231660-d42236e9-ceec-46c1-8ace-069d07517b6f.png)

After Log Transformation

![image](https://user-images.githubusercontent.com/85148563/156231681-c54bd7fa-9b72-4870-b348-bb7b8e04543e.png)

# SVD- Singular Value Decomposition

The Singular Value
Decomposition, is a matrix
decomposition method for
reducing a matrix to its
constituent parts in order to
make certain subsequent
matrix calculations simpler. It
provides another way to
factorize a matrix, into singular
vectors and singular values.

# Machine Learning Algorithm:

**Collaborative Recommendation System

No of Components in SVD = 35

Pivot Matrix: Shape (22363,12101)

![image](https://user-images.githubusercontent.com/85148563/156231868-923d1c8b-1984-484c-9299-c8f14e317afe.png)

**Evaluation for Collaborative Filtering

recall@5: 0.3847

recall@10: 0.4759

recall@15: 0.5358

**Content Based Recommendation System

![image](https://user-images.githubusercontent.com/85148563/156232003-4ae1f2aa-218e-486f-be3a-6c488e0f167c.png)
  
**Cosine Similarity

➢
Cosine similarity measures the
similarity between two vectors of
an inner product space.

➢
It is measured by the cosine of
the angle between two vectors
and determines whether two
vectors are pointing in roughly
the same direction.

➢
It is often used to measure
document similarity in text
analysis.

**Evaluation for Content Based Recommendation System

recall@5:0.83814

recall@10:0.8630

recall@15:0.8680

# Conclusion

➢
We got recall@5: 0.3847 and recall@10: 0.4759 for
collaborative Model.

➢
We got recall@5: 0.83814 and recall@10: 0.8630 for
content based Model.

➢
As we can see We are getting better recall value for
content based model than collaborative model.

➢
So we can conclude that content based model is
optimal model for product recommendation.
