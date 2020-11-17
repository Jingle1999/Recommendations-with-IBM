# Recommendations-with-IBM

Recommendations with IBM

I.	Basic Information

I.1 	Introduction

When you walk into a shop the Salesperson talking to you will try to figure out your taste by asking you specific questions like “What do you want to buy? – Our clients currently buy this item the most” or “I saw you bought/watched product A. Maybe you also like product B, which would be like product A, but with more functions, or you also might like product C, which complements product A.” When talking to friends you also hear recommendations about the last purchase they made, that you might like, too.
This process of recommendations will be shown in the following more algorithm-based by using the Python-programming-language. It’s quite similar to what you would expect from real-life recommendations, but less intuitive and more fact-based.
1)	What’s the product people buy the most (top bought, top consumed, top viewed, etc.)?
2)	What’s the item people with a similar taste bought? Are there items which you would like to purchase, when comparing to your consuming behaviour?
3)	What’s the product that you would buy?
4)	Where the recommendations good?
According to McKinsey “35 percent of what consumers purchase on Amazon and 75 percent of what they watch on Netflix come from product recommendations based on (…) algorithms” (https://www.mckinsey.com/industries/retail/our-insights/how-retailers-can-keep-up-with-consumers). Here you see a clear link between recommendations and revenue, as competition on the internet is getting more fierce then ever (please also see https://cloud.google.com/solutions/recommendations-using-machine-learning-on-compute-engine). Hence, let’s check how we can create recommendations to generate revenue.
Before we dig deeper into the specific recommendation task, please find a quick overview over the different recommendation types below.

I.2	Knowledge Based Recommendations

Knowledge Based Recommendations use knowledge about items that meet user specifications to recommend items, e.g. by using filters. Hence, users provide information about the kind of recommendation they’ll expect.

I.3	Collaborative Filtering Based Recommendations

Collaborative Filtering Based Recommendation is the method of making recommendations based on using the collaboration of user-item-interaction; users and items are treated dependent from each other, e.g. model-based and neighbourhood-based collaborative filtering.

I.4	Content Based Recommendations

Content Based Recommendations use information about items to find similarities. Often the similarities are related to item description or purpose, e.g. by creating and using a similarity matrix.

I.5	   Singular Value Decomposition (SVD)

SVD serves for validation purposes of our recommendations and answers the question, if our recommendations where any good. Basically, SVD is about finding latent factors between an item and the recommendation. As a matter of fact, understanding traditional SVD approaches to matrix factorization is useful as a start to several matrix factorization techniques that are possible in practice.
Starting point of the SVD is a user-item-matrix A, which consists of the following (sub-) matrices:
A = U ∑ VT 
with
n = number of users
k = number of latent features used
m = number of items
Matrix	Question to answer	Dimensions
U	How do users feel about latent features?	U = n - k
∑	How much does each latent feature matter in predicting rating?	∑ = m - k
VT	How does a latent feature appear in or rather relate to an item?	VT = k - m

I.6 	The cold start problem

In cases where new users or movies are included, collaborative filtering does not work as technique to predictions. Here you need to use content based or rank based recommendations. 

I.7 To go further

In order to analyse the interactions, that users have with articles on the IBM Watson Studio-platform and make recommendations about new articles they might like, a recommendation system will be built up.

The process for solving this recommendation task involves the following steps:
-	Exploratory Data Analysis
-	Rank Based Recommendations
-	User-User Based Collaborative Filtering
-	Content Based Recommendations (according to Natural Language Processing, NLP)
-	Matrix Factorization (setting-up a Machine Learning-environment for prediction-purposes)



