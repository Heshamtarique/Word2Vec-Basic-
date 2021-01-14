# Word2Vec-Basic-
10th jan 2021. 
Distributionalal semantic is one of the most successful idea in statistical NLP. In this repository we dicussed a basic model "Word2Vec". which represent any word in the form of vectors of dimension given by the user.
word2vec (A framework for learning word vectors) has two types:- 
1- skip gram  (given the target word predicting the context word)
2- continous Bag of words (given the context word predicting the target word)

word vectors are generally called as "WORD EMBEDDING", Graphical data:- typically we use 50, if using laptop make it to 300, for maximum performance make it to 2000 or 4000.
we can see some morphological forms are grouped together, as its very high dimension so its tough to visualize so we map it to 2D 
Algorithm:-
Start with random vector, itearte through each position, somehow a miracle occur and we have a word vector space. Now try to make prediction and see how well we can predict and then change the vector representation of words in a way that we make the prediction better.

# PROBABILISTIC MODEL OF WORD2VEC
1: for each position t = 1, 2.....,T, predict centre word within a window of fixed size m. given center word (w)j.     this is calculated using Likelihood equation, theta (parameter)
2: Now we define a cost function - average negative log likelihood. and this cost function is minimised to get the vector space.
3: A prediction function is defined using two vectors per word. (v)w when w is center word and (u)w  when w is context word. 
now we can use any function such as SOFTMAX function --- which maps arbitrary function (x)i to a probability distribution (P)i. 'max' beacuse amplifies probability of largest (x)i.  'soft' beacause still assigns some probability to smaller (x)i. This is frequently used in Deep Learning. 

