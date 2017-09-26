# Machine Learning Basic Understanding

## Introduction

### Machine Learning [INCLUDE LEARNING FLOW]

General Machine learning definition would be the way to make computers learn how to perform non-linear or complex tasks that even humans cannot be easily describe, or even don't know how to accomplish.

Machine Learning is one of the broad subfield of computer science artificial intelligence (AI) that focus on the design system that can learn and make decisions and prediction, it works with processing data to find the patterns of related data information and later to be used to analyse new data and make decisions based on the result of the data provided before, this means, the larger the data collection that the machine could learn, the better it will perform. Machine learning most of the time relies on specific 'features' of the data that are understandable for a computer. For example of that explanation is, say we are talking about text, text would contains words, length of overall text and even for each word, word could be categorised on negative, positive or even emotional type of words. The process of collecting features is called 'features extraction'.

### Types of Machine Learning

There are several categories for Machine Learning classifier, but there are three main classifier that are commonly be used, all three will be explained below.

#### Supervised Machine Learning classification

Supervised Machine Learning classification relies on the data that are labelled on its category or class (pre-defined datasets), it's trained using 'guided' data, this explanation will explain what it means. Say we want our machine to differentiate picture of humming-bird and ostrich, we first provide many pictures of humming-bird and ostrich with correct label on them, so that the computer knows where to classify them, and it will learn the 'features' of the images and later it will be able to differentiate 'unseen' images whether the images is closer to ostrich or to humming-bird.

#### Unsupervised Machine Learning classification

Unsupervised Machine Learning classification is about the same with Supervised Machine Learning classification, it's just the 'label' from before is not provided, letting the computer learn by itself from the large amount of characteristics and data provided. For example, we want the computer categorise humming-bird and ostrich, but we forgot to give the correct lable on it. The computer will learn the datasets so fit the requirements (2 types of picture, humming-bird and ostrich) by itself using technique called clustering, it will differentiate the features it has collected to separate the 2 different groups based on some inherent features or characteristics of the pictures.

#### Reinforcement learning

Last but not least mainly used learning method is Reinforcement learning. This learning method is used for something that's impossible to calculate because the possibility is way too many. As an example, say the computer want to learn how to play chess. As an input to this learning problem, we told the Machine Learning whether the game that is going to be learned result was won or lost, so the computer doesn't have 'labeled' move yet, but it has the result of the outcome of the game. With this knowledge the Machine Learning algorithm can play a lot of games and each of the time, the moves that resulted in a winning combination will get a bigger 'weights'.

## Common terminology related to Machine Learning

*Classification* within the machine learning is the sub-category of supervised learning where computational classification models or “classifiers” are built to assign objects into finite number of class labels. The object is also called as ‘input’ which is taken into the process of classification. There are two types of classification which is binary classification and multi-class classification. Binary classification has only 2 class labels that either means ‘yes’ or ‘no’ but is written in another way with connection to the topic or subject of the input that is being classified. Aside from that, there is the multi-class classification which assigns more than 2 class labels or description that is related to the subject of the input being classified.

Furthermore, *regression* is where a computational model is built to predict values of some continuous response variable. Regression is also a sub-category of supervised learning. In addition, the labels are associated with continuous real values where the arrangement does not matter but the value does. Examples of implementation of regression in real life is house price prediction, stock price, climate, oil price, finance, epidemiology and temporal trends such as temperature and weather. Regression is basically understood as a system to answer questions such as “How much?” or “How many?”.

*Decision tree* in machine learning is a tool used to visually or explicitly support decisions. Tree-like graphs or models of decisions and their possible consequences are used within this method. Moreover, this tool is generally used in data mining to derive strategy to reach a certain goal or task completion. A basic example is such as the usage of titanic data set to predict whether a passenger will survive or not. The model uses features, attributes and columns from the data set. A decision tree is drawn upside down with it’s root at the top. On the other hand, the feature importance in the decision tree is clear and relations can be viewed easily.

In machine learning, *generative model* (graphical) is used in probability and statistics to generate data values with some parameters hidden. Generative model uses direct data modeling as an intermediate step to from conditional probability density function. Such models are mixture model, directed graphical model and undirected graphical model. Within the generative modeling, input data (x) is classified into labels (y) where x and y are any names of data. Generative model learns the **joint** probability distribution *p (x.y).*

*Discriminative model* however is where input data (x) that is classified into labels (y) where x and y are any names of data learns the **conditional** probabilty distribution *p (x|y)* which should be read as “the probability of y given x”. Discriminative models are also referred to as conditional models to model the dependence of variable y on a variable x. It is often used in supervised learning such as in logistics, Regression, SVMs and Neural Networks.Examples of discriminative models are support vector machine, mapped data and separating hyperplane.


## Statistical Classification //+

--- //+ [PARAPHRASE]
In machine learning and statistics, classification is the problem of identifying to which of a set of categories (sub-populations) a new observation belongs, on the basis of a training set of data containing observations (or instances) whose category membership is known. An example would be assigning a given email into "spam" or "non-spam" classes or assigning a diagnosis to a given patient as described by observed characteristics of the patient (gender, blood pressure, presence or absence of certain symptoms, etc.). Classification is an example of pattern recognition.

In the terminology of machine learning,[1] classification is considered an instance of supervised learning, i.e. learning where a training set of correctly identified observations is available. The corresponding unsupervised procedure is known as clustering, and involves grouping data into categories based on some measure of inherent similarity or distance.

Often, the individual observations are analyzed into a set of quantifiable properties, known variously as explanatory variables or features. These properties may variously be categorical (e.g. "A", "B", "AB" or "O", for blood type), ordinal (e.g. "large", "medium" or "small"), integer-valued (e.g. the number of occurrences of a particular word in an email) or real-valued (e.g. a measurement of blood pressure). Other classifiers work by comparing observations to previous observations by means of a similarity or distance function.

An algorithm that implements classification, especially in a concrete implementation, is known as a classifier. The term "classifier" sometimes also refers to the mathematical function, implemented by a classification algorithm, that maps input data to a category.

Terminology across fields is quite varied. In statistics, where classification is often done with logistic regression or a similar procedure, the properties of observations are termed explanatory variables (or independent variables, regressors, etc.), and the categories to be predicted are known as outcomes, which are considered to be possible values of the dependent variable. In machine learning, the observations are often known as instances, the explanatory variables are termed features (grouped into a feature vector), and the possible categories to be predicted are classes. Other fields may use different terminology: e.g. in community ecology, the term "classification" normally refers to cluster analysis, i.e. a type of unsupervised learning, rather than the supervised learning described in this article.
--- //+

Statistical classification models the class as a random variable and uses its distribution to perform classification, is basically annotated like this:

	**p(y|x)**
	this is a conditional probability of class y given measurement x

Where:
- p = probability
- y = class/category
- x = measurement/features (that differentiate one class/category with others)

#### Empirical Risk Minimization

Resources:
https://en.wikipedia.org/wiki/Empirical_risk_minimization

### What is ML used for?

Machine Learning strongly rely on data, the main requirement of using Machine Learning is having a data for training the model. The amount of the data depends on what one's trying to achieve, how complex the problem is. However, more data to supply to the machine is always better, this will make the prediction more accurate and trained the computer even more. One note for this, the data that are provided to train the model should be similar with the new 'unknown' data that are going to make a prediction on later. As an example, if you want to predict the opinions of audience about some movies, it's best to use resources (data) from movies reviews as well, and it may yield not really great results if the reviews of the food was applied instead. But when we know what we're trying to achieve, Machine Learning could be the answer that we're looking for, as it has been at the center of many technological advancements in recent years (speech recognition systems, computer vision recognition systems, self-driving cars or even complex game bots).

### State-of-the-art classifiers

[ON HOLD]

### Using a Machine Learning classifier [MERGE]

- Training: train all the trainable parameters of your classifier using the training set (dataset) to form a model and later to be used for prediction
- Testing / Predicting: measure the accuracy of your classifier (generated model) using a separate test set (the data that is not used for model training)
- Choose the non-trainable parameters (aka "hyperparameters") empirically, using the test set or even better, use a separate validation set

# Deep learning [INCLUDE LEARNING FLOW]

A subfield of machine learning that often uses algorithms which are inspired by artificial neural networks to generate models is the *deep learning*. Deep learning also utilizes a mathematical model to construct large neural networks that focuses on scaling and training the network with more data to increase their performance. A benefit of deep learning is their ability to automate extraction of features from raw data which can also be called as ‘feature learning’. Deep learning also excels in problem domain where inputs and outputs are analog. This means that they are not in small quantity such as in tabular format. Instead, the inputs and outputs are images of pixel data, files of audio data as well as documents of text data.

Additionally, *neural networks or artificial neural networks* are also part of machine learning. It is a network of interconnected nodes that makes up a model. Neural networks is also described as a biologically-inspired programming paradigm which enables computers to learn from observational data. Neural networking is used to estimate or approximate functions that depends on a large number of input. Due to it’s ability to withstand large number of inputs, it is commonly used when volume of inputs are too large for a standard machine to overcome. Neural networks are the best solution to problems in image recognition, speech recognition and natural language processing.

## Deep Learning - The Chain rule

Resources:
- https://www.youtube.com/watch?v=fDeAJspBEnM

## NLP (Natural Language Processing)

Resources:
- https://www.quora.com/In-what-order-should-I-learn-machine-learning-deep-learning-natural-language-processing-and-artificial-intelligence
- http://blog.aylien.com/10-common-nlp-terms-explained-for-the-text/

## LSTM (long short-term memory)

Resources:
- https://deeplearning4j.org/lstm.html
- https://medium.com/@shiyan/understanding-lstm-and-its-diagrams-37e2f46f1714


## About Tensorflow

TensorFlow is essentially a framework for building Deep Learning Neural Networks provided by Google Brain team, it's an open source project since November 2015, however, there's something to note, Google didn't release any of its trained models, they just release the 'engine' of it. Because as explained before, it takes a large amount of data and computing resources to train a Deep Learning model. The trained model is what enables the impressive pattern recognition or prediction capabilities.
TensorFlow is feature rich framework, as it's designed to be a library that are capable on doing Complex Numerical Computation to build machine learning models from scratch. It has its own scikit-learn like for high level machine learning API, it's called scikit-flow.
Tensorflow uses Directed Graph as its computational model, the functions itself are nodes & edges data, this what makes it stand on the right place for deploying Neural Networks and also it makes TensorFlow easily distributed across CPUs, GPUs and even multiple system environments. This is one of the advantage of TensorFlow, the flexibility on distributed environments.
TensorFlow also able to run under some supporting environments, like Keras or Tensorboard. Tensorboard is a visualization software for tensorflow, it enables easier debugging and analyzing machine learning models.
Pre-trained tensorflow model also able to run with small computing resources like mobile, raspberry pi, etc. makes it highly portable.
Also last but not least, TensorFlow is used by many companies when they adopt Deep Learning for their systems.

## BiMPM short Explanation

Resources:
- https://web.stanford.edu/class/cs224n/reports/2748045.pdf
- https://github.com/bradleypallen/keras-quora-question-pairs
