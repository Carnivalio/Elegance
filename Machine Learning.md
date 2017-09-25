# Machine Learning Basic Understanding

## Introduction

What is machine learning?

- https://www.quora.com/What-is-machine-learning-4
- http://nkonst.com/machine-learning-explained-simple-words/

## Machine Learning Basic

Statistical Classification

- https://en.wikipedia.org/wiki/Statistical_classification
https://www.quora.com/What-is-the-difference-between-deep-learning-and-usual-machine-learning

Statistical classification models the class as a random variable and uses its distribution to perform classification, is basically \\+annotated like this:

p(y|x)

Where:
p = probability
y = class/category
x = measurement/features (that differentiate one class/category with others)

this is a conditional probability of class y given measurement x

- maximum-a-posteriori decision rule

- minimum theoretical misclassification error rate
	- minimum risk or minimum expected loss
	- Minimum risk decision rule

- https://en.wikipedia.org/wiki/Empirical_risk_minimization
- https://stats.stackexchange.com/questions/272411/why-is-empirical-risk-minimization-prone-to-overfitting

State-of-the-art classifiers
• No classifier has reported higher empirical accuracy than all others over all test sets
• A non-exhaustive list of empirically-reputed classifiers:
	• the support vector machine (SVM)
	• artificial neural networks (ANN), including deep neural networks (DNN)
	• k nearest neighbours (kNN)
	• decision trees and random forests
	• AdaBoost
• Try them in WEKA (University of Waikato, NZ)
https://www.quora.com/What-are-the-state-of-the-art-algorithms-in-Machine-Learning

https://en.wikipedia.org/wiki/Outline_of_machine_learning

Using a classifier
• Training: train all the trainable parameters of your classifier using the training set
	• In the case of Bayesian classification, you will have to train the prior probability p(y), and one likelihood p(x|y) for every value of y (every possible class)
• Testing: measure the accuracy of your classifier using a separate test set
• Choose the non-trainable parameters (aka “hyperparameters”) empirically, using he test set or a separate validation set (better)

# Deep learning + basic scheme
https://www.forbes.com/sites/quora/2016/09/23/what-are-the-differences-between-ai-machine-learning-nlp-and-deep-learning/#181507e4274f
https://www.quora.com/What-is-deep-learning-Why-is-this-a-growing-trend-in-machine-learning-Why-not-use-SVMs

# About Tensorflow
https://www.quora.com/What-is-TensorFlow-1
https://www.quora.com/What-can-TensorFlow-do

# Deep Learning - The Chain rule
https://www.youtube.com/watch?v=fDeAJspBEnM

# NLP (Natural Language Processing)
https://www.quora.com/What-is-natural-language-processing-in-laymans-terms

https://www.quora.com/In-what-order-should-I-learn-machine-learning-deep-learning-natural-language-processing-and-artificial-intelligence

# Bidirectional LSTM (long short-tem memory)
https://www.quora.com/What-is-LSTM
https://www.quora.com/How-does-bidirectional-LSTM-RNN-work-on-recognition-text
https://www.quora.com/When-should-one-use-bidirectional-LSTM-as-opposed-to-normal-LSTM

# BiMPM short Explanation
https://web.stanford.edu/class/cs224n/reports/2748045.pdf
https://github.com/bradleypallen/keras-quora-question-pairs

## Readings
- http://blog.aylien.com/10-machine-learning-terms-explained-in-simple/
- http://www.huffingtonpost.com/quora/machine-learning-simply-e_b_12589446.html
- http://nkonst.com/machine-learning-explained-simple-words/
- https://www.analyticsvidhya.com/blog/2015/06/machine-learning-basics/
- https://www.quora.com/What-is-machine-learning-4
- https://www.google.com.au/search?q=easy+explanation+of+machine+learning+quora&oq=easy+explanation+of+machine+learning+quora&gs_l=psy-ab.3..33i21k1.28799.30502.0.30661.6.6.0.0.0.0.226.413.0j1j1.2.0....0...1.1.64.psy-ab..4.2.412...33i22i29i30k1.0._DPv_WDFz_g
- https://raw.githubusercontent.com/bradleypallen/keras-quora-question-pairs/master/quora-q-pairs-model.png
- https://www.datacamp.com/community/tutorials/data-science-industry-infographic
