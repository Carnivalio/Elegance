## Machine Learning

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

### Other Common terminology related to Machine Learning

Furthermore, *regression* is where a computational model is built to predict values of some continuous response variable. Regression is also a sub-category of supervised learning. In addition, the labels are associated with continuous real values where the arrangement does not matter but the value does. Examples of implementation of regression in real life is house price prediction, stock price, climate, oil price, finance, epidemiology and temporal trends such as temperature and weather. Regression is basically understood as a system to answer questions such as "How much?" or "How many?".

*Decision tree* in machine learning is a tool used to visually or explicitly support decisions. Tree-like graphs or models of decisions and their possible consequences are used within this method. Moreover, this tool is generally used in data mining to derive strategy to reach a certain goal or task completion. A basic example is such as the usage of titanic data set to predict whether a passenger will survive or not. The model uses features, attributes and columns from the data set. A decision tree is drawn upside down with it's root at the top. On the other hand, the feature importance in the decision tree is clear and relations can be viewed easily.

In machine learning, *generative model* (graphical) is used in probability and statistics to generate data values with some parameters hidden. Generative model uses direct data modeling as an intermediate step to form conditional probability density function. Such models are mixture model, directed graphical model and undirected graphical model. Within the generative modeling, input data (x) is classified into labels (y) where x and y are any names of data. Generative model learns the **joint** probability distribution *p (x.y).*

*Discriminative model* however is where input data (x) that is classified into labels (y) where x and y are any names of data learns the **conditional** probability distribution *p (x|y)* which should be read as "the probability of y given x". Discriminative models are also referred to as conditional models to model the dependence of variable y on a variable x. It is often used in supervised learning such as in logistics, Regression, SVMs and Neural Networks.Examples of discriminative models are support vector machine, mapped data and separating hyperplane.

### (Statistical) Classification

Statistical Classification in machine learning is used to identify the problem of a set of classes (catgories or sub-populations) where a new observation belongs, based on the training set of data containing instances (or observations) which the category membership is known. [REFER TO ML TYPES]

Most of the time, the observations are analyzed individually into a set of quantifiable properties, known variously as features. There are various type of the properties, such as:
- Categorical (e.g. "A", "B", "AB" or "O", for blood type)
- Ordinal (e.g. "large", "medium" or "small")
- Integer-valued (e.g. the number of occurrences of a particular word in an email)
- Real-valued (e.g. a measurement of blood pressure)

While *Classification* within the machine learning (specifically) is the sub-category of supervised learning where computational classification models or "classifiers" are built to assign objects into finite number of class labels. The object is also called as 'input' which is taken into the process of classification. There are two types of classification which is binary classification and multi-class classification. Binary classification has only 2 class labels that either means 'yes' or 'no' but is written in another way with connection to the topic or subject of the input that is being classified. Aside from that, there is the multi-class classification which assigns more than 2 class labels or description that is related to the subject of the input being classified.

Statistical (machine learning) classification models the class as a random variable and uses its distribution to perform classification, is basically annotated like this:

	*p(y|x)*

	this is a conditional probability of class y given measurement x

Where:
- p = probability
- y = class/category
- x = measurement/features (that differentiate one class/category with others)

### Maximum A Posteriori Estimation

Maximum a posteriori (MAP) estimation is the value of the parameter that maximizes the entire posterior distribution (which is calculated using the likelihood). A MAP estimate is the mode of the posterior distribution. In Machine Learning world, the maximum a posteriori estimation can be used for optimization of the decision.

MAP explained using an analogy:
- Prior: Given everything you knew about machine learning so far up to this point
- Data: Everything you've seen here in the document
- Maximum estimation (guess): the 'best' guess of your understanding about machine learning (that are in scope of this document)
- Posteriori: Your best guess given all that you know up to this point

### Machine Learning Usage

Machine Learning strongly rely on data, the main requirement of using Machine Learning is having a data for training the model. The amount of the data depends on what one's trying to achieve, how complex the problem is. However, more data to supply to the machine is always better, this will make the prediction more accurate and trained the computer even more. One note for this, the data that are provided to train the model should be similar with the new 'unknown' data that are going to make a prediction on later. As an example, if you want to predict the opinions of audience about some movies, it's best to use resources (data) from movies reviews as well, and it may yield not really great results if the reviews of the food was applied instead. But when we know what we're trying to achieve, Machine Learning could be the answer that we're looking for, as it has been at the center of many technological advancements in recent years (speech recognition systems, computer vision recognition systems, self-driving cars or even complex game bots).

### Machine Learning Classifiers

There are no 'one for all' solution in Machine Learning, there are uncountable probability of solution out there, so it's hard to define the best way to solve multiple problems with same approach, it is required to set the constraints of the model that we are trying to achieve when we talk about Machine Learning. But, there are some very well-performed algorithms on some use-cases for their suitable area, such as:
- Artificial Neural Networks (ANN): highly customizable and also gives a very good result. (including Deep Neural Networks (DNN))
- Support Vector Machine (SVM) + kernels: enhanced version of Neural Network with good performance with its ease of use, easy to customize.
- Decision Tree: overall speed is very fast, rule based, inheritable but highly unstable
- Random Forests: lots of 'trees' created with sampled data, also it has a high learning rate (with enough number of training instances).
- AdaBoost: weak classifiers ensembled together to form a boosting approach.

#### Using a Machine Learning Classifier

- Training: train all the trainable parameters of your classifier using the training set (dataset) to form a model and later to be used for prediction
- Testing / Predicting: measure the accuracy of your classifier (generated model) using a separate test set (the data that is not used for model training)
- Choose the non-trainable parameters (aka "hyperparameters") empirically, using the test set or even better, use a separate validation set

## Deep learning

A subfield of machine learning that often uses algorithms which are inspired by artificial neural networks to generate models is the *deep learning*. Deep learning also utilizes a mathematical model to construct large neural networks that focuses on scaling and training the network with more data to increase their performance. A benefit of deep learning is their ability to automate extraction of features from raw data which can also be called as 'feature learning'. Deep learning also excels in problem domain where inputs and outputs are analog. This means that they are not in small quantity such as in tabular format. Instead, the inputs and outputs are images of pixel data, files of audio data as well as documents of text data.

Additionally, *neural networks or artificial neural networks* are also part of machine learning. It is a network of interconnected nodes that makes up a model. Neural networks is also described as a biologically-inspired programming paradigm which enables computers to learn from observational data. Neural networking is used to estimate or approximate functions that depends on a large number of input. Due to it's ability to withstand large number of inputs, it is commonly used when volume of inputs are too large for a standard machine to overcome. Neural networks are the best solution to problems in image recognition, speech recognition and natural language processing.

### NLP (Natural Language Processing)

*Natural Language Processing (NLP)* is a computer science and method of communicating within artificial intelligence and computational linguistics. It utilize an intelligent system that uses a natural language such as English which enables interactions between computers and human/natural language. At the same time, NLP focuses on the machine’s ability to understand or mimic the understanding of human language. Furthermore, NLP is where a computer interacts by understanding, analyze,  manipulating and derive human language to perform task such as speech recognition, language translation, text classification, automatic summarization, conversational agents, sentiment analysis, information extraction, co-reference resolution and named entity extraction, and sentence segmentation. The input and output of NLP can be in speech or text.

 On the other hand, NLP’s components includes the *Natural Language Understanding (NLU)* and *Natural Language Generation (NLG)*. The NLU is where the the NLP mapping a given input (natural language) into useful representations. Besides that, the NLU also analyzes different aspects of the human language. The NLG however, involves the process of producing meaningful sentences and phrases in the form of natural language from internal representation. The NLG includes *text planning* (retrieving relevant content from knowledge base), *sentence planning* (required words are chosen to form meaningful phrases), and *text realization* (mapping sentence plan into sentence structure). In addition, the NLU is harder than NLG due to NLU having difficulties such as, the presence of extremely rich from and structure that are ambiguous. The NLU’s level of ambiguity is lexical, syntax, and referential. NLU can either have one input that mean different things or many inputs that means the same thing.

Aside from that, NLP has terminologies such as phonology, morphology, morpheme, syntax, semantics, pragmatics, discourse, and world knowledge. NLP is beneficial to be used in companies to improve efficiency of documentation, and identify most pertinent information from huge databases. Real NLP applications generally perform tasks using two families of approaches which is *symbolic* and *statistical*. The symbolic approach contains a set of rules that are usually hand-written but sometimes automatically learned. It is easier to be understood by a human. In the symbolic approach, humans have better control of the methods such as deleting, changing and creating rules. However, statistical approach typically uses machine learning algorithms to learn language phenomena. Although, this approach has it’s limitations such as the 5% error rate of the HMM-based PoS taggers. Without NLP, artificial intelligence can only understand the meaning of language and answer basic questions but is unable to understand the meaning of words in context.

In NLP, we have the *Information Extraction* is a task involving topics such as text understanding and machine learning. Apart from that, structured information is extracted from an unstructured and/or semi-structured machine-readable source such as text document or web pages. In order to be able to use and apply information extraction, familiarity with linear algebra, probability, and basic knowledge of machine learning is needed. Coding skills are also needed for this task such as in Python, Lua, Java, C++ and Scala programming languages. Information extraction processes large body of texts in order for it to be inscribed into relational database or analyzed using data mining. In this matter, body is text is the input whereas the output is a closely defined (rigid) data format that means only a fraction of the data is relevant. The accuracy of this method such as on the information extraction software; MUC-6, the data set has 75% precision and 75% recall based on forum of The Message Understanding Conference sponsored by DARPA.

Moreover, NLP involves *Named Entity Recognition (NER)* is the subtask in information extraction where name entities in computer-readable text (words/phrases) via annotation with categorization tags are being identified and classify them in to groups. It’s vital role is in many disambiguations such as the reference resolution, and meaning representation in human language processing applications. This type of tagging can be use to extend semantic parsers, part-of-speech taggers and thematic meaning which will produce better results. The three top-level category in named entity recognition is entity names, temporal expressions and number expressions. NER requires some key design decision such as the chunking and text representation, inference and ambiguity resolution algorithms, implementation of external knowledge resources, and modeling of non-local dependencies. On top of that, NER is applied in task such as question answering or machine translation by way of ‘indexing’ to precisely find documents related to the groups of words/phrases belong in which improves their results.

Besides that, there is the *Corpus (literally Latin for body)* or *Corpora* which is a large collection of documents/texts to perform tasks such as statistical analysis and hypothesis testing. Such collections of texts can be formed from single or multiple languages. It can also be used infer and validate linguistic rules. Other than that, the corpus is either open or closed. Open corpus means that it does not claim to contain every data from a specific area whereas closed corpus claims to contain all or almost all data from a certain field. Corpus is a written or spoken body of material which a linguistic analysis is based on. A corpus is used to provide better descriptions of languages for grammarians or other interested parties regarding computational linguistics.

Subjective extraction of information from a piece of text is called as the *Sentiment Analysis (SA; also known as opinion mining)*. Generally, a ‘sentiment’ is where a binary opposition in opinions is assumed. However, ‘sentiment analysis’ is where the NLP, statistics or machine learning is used to extract, identify and characterize a text unit’s sentiment content. Furthermore, task that can be performed by using the sentiment analysis is summarization, information extraction and “flame” detection. In addition, the SA is also used TO discard subjective information and for bias identification in news sources such as within the BBD or CNN. Applications of SA is commonly used branches like in politics, law, sociology and psychology

*Word Sense Disambiguation (WSD)* or *Lexical Ambiguity Resolution* in NLP is the capability to identify meaning of words in a context using computational methods. The third party that is incorporated within this task is the Corpus or knowledge base such as SkELL, Voyant Tools, Wikipedia, WordSmith or Sketch engine. Apart from that, the ambiguity of WSD is related to the polisemy of words where isolated words are ambiguous. The WSD is useful in performing potential intermediate tasks for many NLP systems including information extraction, machine translation or NLU. Typically, WSD involves two task which are, determining the different possible senses/ meanings of each word, and tagging each word of a text with its appropriate sense with efficiency and high accuracy.

NLP also includes the *Bag of Words (BoW)* which is a model that is commonly used in text classification. It focuses on categorization of documents. Also, by matching different categories, BoW can be used to identify where a certain block of data came from. Other than that, BoW is generally just a tool to convert text documents into a vector that describes it’s feature and contents. The BoW model had texts that are represented as a multiset of words. Besides that, In BoW, the model would take into account the words and frequency of occurrence in the sentence or the document but pays no attention to wards semantic relationship, grammar and word order in the sentences.

Additionally, in *Explicit Semantic Analysis (ESA)*, it refers to the way of understanding and extracting the meaning from a written text rather than on the surface form of vocabulary of a word or document. The text that is extracted in ESA can either be a single word, a couple of words, a sentence, paragraphs or a whole book. ESA is used in information retrieval, document classification and semantic relatedness calculation. Moreover, ESA could be used a library by making alterations and tweaking to the source code.

### Long short-term memory (LSTM)

One recurrent neural network (RNN) architecture that remembers values over arbitrary intervals is called Long short-term memory (LSTM). Stored values stays as it is as learning proceeds, it doesn't change. RNNs allow both ways, forward and backward connections between neurons to help preserving the error that can be backpropagated through time and layers. It's opening a channel to link causes and effects remotely by allowing recurrent nets to continue learning over many (over 1000) time steps by maintaining more constant errors.

A gated LSTM cell contains information outside the normal flow of the recurrent network. Like handling a computer's memory, information can be read from, written to, or stored in a cell. Using the gates that open and close, LSTM cell decides on what to store, and when to allow reads, writes and erasures. These LSTM gates are analog, unlike digital storage on computer, it's deployed with element-wise multiplication using sigmoids, which are all in the range of binary (0 or 1). The advantage of using analog instead of digital is it's more differentiable, thus suitable for backpropagation.

An LSTM is well-suited to classify, process and predict, well-suited to learn from experience to classify, process and predict time series with time lags of unknown size and duration between certain important events. The advantage to LSTM over alternative RNNs is its relative insensitivity to gap length.

### About TensorFlow

TensorFlow is essentially a framework for building Deep Learning Neural Networks provided by Google Brain team, it's an open source project since November 2015, however, there's something to note, Google didn't release any of its trained models, they just release the 'engine' of it. Because as explained before, it takes a large amount of data and computing resources to train a Deep Learning model. The trained model is what enables the impressive pattern recognition or prediction capabilities.

TensorFlow is feature rich framework, as it's designed to be a library that are capable on doing Complex Numerical Computation to build machine learning models from scratch. It has its own scikit-learn like for high level machine learning API, it's called scikit-flow.

Tensorflow uses Directed Graph as its computational model, the functions itself are nodes & edges data, this what makes it stand on the right place for deploying Neural Networks and also it makes TensorFlow easily distributed across CPUs, GPUs and even multiple system environments. This is one of the advantage of TensorFlow, the flexibility on distributed environments.

TensorFlow also able to run under some supporting environments, like Keras or Tensorboard. Tensorboard is a visualization software for tensorflow, it enables easier debugging and analyzing machine learning models.

Pre-trained tensorflow model also able to run with small computing resources like mobile, raspberry pi, etc. makes it highly portable.
Also last but not least, TensorFlow is used by many companies when they adopt Deep Learning for their systems.

### BiMPM Short Explanation

**[TODO: 1]**

Resources:
- https://web.stanford.edu/class/cs224n/reports/2748045.pdf
- https://github.com/bradleypallen/keras-quora-question-pairs
