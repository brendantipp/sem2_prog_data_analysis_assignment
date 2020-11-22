
#  Semester 2 - Programming for Data Analysis Assignment

## Brendan Ryan, GMIT Student - November 2020


### Details of Git Repository

The repository for the assignment and all the files are located here https://github.com/brendantipp/sem2_prog_data_analysis_assignment

### Assignment Details and the Tasks for this assignment 

1. Explain the overall purpose of the numpy.random package
2. Explain the use of the "simple random data" and "Permutations" functions
3. Explain the use and purpose of at least five "Distribution" functions
4. Explain the use of seeds in generating pseudorandom numbers

Please note: My initial project plan for this assignment along with references and research links used can be found at the end of this README

### Software used

- Annacoda distribution package (Python, Git) - www.anaconda.com
- Jupyter Notebook - www.jupyter.org
- cmder - www.cmder.net
- Github www.github.com


### How to run or view the Jupyter Notebook

- The Jupyter notebook can be viewed on my My repository is held on GitHub - ttps://github.com/brendantipp/sem2_prog_data_analysis_assignment

- You can also download and run the Jupyter notebook from the repository to your local hard drive and open with Jupyter Notebooks - www.jupyter.org



### Important changes made to the Numpy.random package and why these changes are important  to software developers

At the time of writing this assignment them most uptodate version of the Numpy module is v 1.19. It is important to note that the latest versions of the Numpy.random package contain updated functions.  In particular there has been some major changes to the Simple Random Data functions - some of the old functons were almost duplicates of each other and were essentially the same function. The Distributions and Permutation functions are very similar in both the new and older versions of the Numpy.random package

It is the job of a software developer to keep up to date with these changes and to maintain their code. In the case of the numpy.random library developers can find the most recent documentation available at https://numpy.org/doc/stable/



## Jupyter Notebook Contents

In the Jupyter Notebook with file name explaining.numpy.random.ipynb I give an overview of the following:

1. An overview of Numpy and the Numpy.random package in Python and their purpose
2. I will explain the use of the "Simple random data" and "permutations" functions
3. I will explain the use and purpose of at least five "Distributions" functions
4. I will explain the user of Seeds in generating pseudorandom numbers.


#### Libraires/Packages used
I will be using the numpy.random package from python and I will also be utilising the Matplotib and Seaborn packages for better visualisation using graphs. 


## Below is a walkthrough of what is contained in the Jupyter Notebook.

### Explain the use and purpose of the numpy.random package https://numpy.org/

In this section of the Jupyter notebook I give an overview of what Numpy is.

NumPy is a python library used for working with arrays, it was created in 2005 by Travis Oliphant. It is an open source project and you can use if freely, NumPy stands for Numerical Python.

NumPy is the fundamental package for scientific computing in Python. It is a Python library that provides a multidimensional array object, various derived objects (such as masked arrays and matrices), and an assortment of routines for fast operations on arrays, including mathematical, logical, shape manipulation, sorting, selecting, I/O, discrete Fourier transforms, basic linear algebra, basic statistical operations, random simulation and much more.


The jupyter notebook outlines how to import numpy and give it a shortened name for ease of use

    #we can import the numpy module as follows using np to give a shortened name to the package for ease of use
    import numpy as np
    print (np.version.version)
  
 
###  1. Overview of the numpy.random package

NumPy offers the random module to work with random numbers - numpy.random is a subpackage of Numpy and is available in the numpy library. We use Numpy.random when we want to generate simulated random data, (pretend data) very useful to programmers when they want to generate some random numbers that follow a certain pattern and also to test their code.

The Numpy.random module contains the functions which are used for generating random numbers. The module contains some simple random data generation methods, some premutation and distribution functions , and random generator functions.

- In this section of the Jupyter Notebook I give an overview of the numpy.random package and why it is so widely used.
- I go into more detail on the numpy.random sub package
- I explain how we load the numpy library into our code


### 2 .  I explain the use of the Simple random data" and "Permutations" functions


#### Simple random data functions

These functions allow us to define sequences and arryas of integers  random real values, choice to generate a random sample from a give 1 dimensional array and bytes to return random bytes. It is worth noting the simple random data functions have been revised and condensed in the newer version of the numpy.random package.

The following are the Simple random data functions

1.  integers - allows us to define a sequences and arrays of integers
2.   random - return random floats between 0.0 and 1.0
3.  choice - to generate a random sample from a given 1 dimensional array
4.  bytes - to return random byte

In my Jupyter notebook I go through each of the above with example(s), for the choice function I give an exmaple of this function can be used to generate six random numbers for a lottery.

#####  Default generator 

Best practice in Numpy version 1.19 and greate is to use Random Generator and the steps are outlined in the Jupyter Notebook.

    # The function numpy.random.default_rng will instantiate a Generator with numpy’s default BitGenerator.
    https://numpy.org/devdocs/reference/random/generator.html#numpy.random.default_rng
    rng = np.random.default_rng()


#### Permutations Functions

There are two permutation functions that are available to us and these provide for random shuffling of data 

- shuffle()
- permutation()

Shuffle function - modifies a sequence in place by shuffling its contents 
permutation function - always returns a shuffled version of the original sequence

In my Jupyter notebook I go through each of the two examples to test how they work in more detail with examples. 


### 3. Distribution Functions 

In this section of the Jupyter notebook I will explain Data Distribution and Data Distribution functions

What is Data Distribution?

Data Distribution is a list of all possible values, and how often each value occurs. Such lists are important when working with statistics and data science. The random module offer methods that returns randomly generated data distributions.

I explain the purpose and use of the following 5 Distribution functions available in numpy.random


#### Normal Distribution 

The Normal Distribution is one of the most important distributions. It is also called the Gaussian Distribution after the German mathematician Carl Friedrich Gauss. It fits the probability distribution of many events, eg. IQ Scores, Heartbeat etc. The curve of a Normal Distribution is also known as the Bell Curve because of the bell-shaped curve. In the Jupyter notebook I give examples of how this distribution works and where it can be used.


#### Uniform Distribution

The uniform distribution defines equal probability over a given range for a continuous distribution. For this reason, it is important as a reference distribution. One of the most important applications of the uniform distribution is in the generation of random numbers. It is used to describe probability where every event has an equal change of occurring for example as in the generation of random numbers. In the Jupyter notebook I give examples of how this distribution works and where it can be used 


#### Logistic Distribution

Logistic Distributions help us in describing the statistical growth of the data. It is known for predicting how the growth will happen by taking in certain data. In the Jupyter notebook I give examples of how this distribution works and where it can be used. I also go through the difference between a Logistic and Normal Distribution with graphed examples.


#### Binomial Distribution

A binomial distribution can be thought of as simply the probability of a SUCCESS or FAILURE outcome in an experiment or survey that is repeated multiple times. The binomial is a type of distribution that has two possible outcomes (the prefix “bi” means two, or twice). 

In the Jupyter notebook I give examples of how this distribution works and where it can be used. I go through the differences between a Normal and Binomial Distribution with graphed examples.


### 4. Explaining the use of Seeds in generating Pseudorandom Numbers

In this section of my Jupyter notebook I attempt to explain the fundamental problem when using computers to simulate or work with random processes. I explain how Computers need some sort of mechanism to generate random number. 
Computers get around this by using pseudo-random number generators.

In order to work properly, pseudo-random number generators require a starting input. We call this starting input a “seed.”.

Why use seeds? - Programmmers would often want to set a seed so that the same range of values etc are returned for testing their conde for consistency 

In this section I outline changes in the new version of the Numpy package version 1.19 and greater. I outline the way of generating seeds has changed from the Merseene Twister method to a new algorithm called PCG64. This new algorithm is called a Permuted Congruential Generator (64 Bit PCG 64)

I researched and outline the reasons why the PCG64 algorithm is better than the previously used Merseene Twister method.

Examples of setting seed using the older and newer methods is included in the notebook. In the exsample coded dont set a seed and then we do , I explain the output of both code examples and the difference setting a seed makes.

### References used and research undertaken as part of my assignment. 

##### Numpy.Random

- https://www.numpy.org
- https://numpy.org/doc/stable/reference/random/index.htm
- https://numpy.org/devdocs/reference/random/generator.html#numpy.random.default_rng
- https://docs.scipy.org/doc/numpy-1.15.1/user/whatisnumpy.html
- https://www.w3schools.com/python/numpy_intro.asp
- https://stackoverflow.com/questions/7029993/differences-between-numpy-random-and-random-random-in-python
- https://numpy.org/devdocs/reference/random/generator.html#numpy.random.default_rng
- https://numpy.org/doc/stable/reference/random/index.html?highlight=random%20sampling%20numpy%20random#module-numpy.random
- https://docs.scipy.org/doc/numpy-1.15.1/user/whatisnumpy.html 
- https://www.javatpoint.com/numpy-random https://realpython.com/python-random

##### Simple random data functions

- https://numpy.org/doc/stable/reference/random/generator.html#numpy.random.Generator
- https://numpy.org/doc/stable/reference/random/generated/numpy.random.Generator.integers.html#numpy.random.Generator.integers
- https://matplotlib.org/
- https://numpy.org/doc/stable/reference/random/generated/numpy.random.Generator.random.html#numpy.random.Generator.random
- https://numpy.org/doc/stable/reference/random/generated/numpy.random.Generator.choice.html#numpy.random.Generator.choice
- https://numpy.org/doc/stable/reference/random/generated/numpy.random.Generator.bytes.html#numpy.random.Generator.bytes


##### Permutations Functions

- The shuffle function (https://numpy.org/doc/stable/reference/random/generated/numpy.random.Generator.shuffle.html#numpy.random.Generator.shuffle)
- The permutaion function. (https://numpy.org/doc/stable/reference/random/generated/numpy.random.Generator.permutation.html#numpy.random.Generator.permutation)
- https://www.w3schools.com/python/numpy_random_permutation.asp


##### Distributions


- https://www.datacamp.com/community/tutorials/probability-distributions-python
- https://www.w3schools.com/python/python_ml_data_distribution.asp
- https://www.statistics.com/glossary/continuous-vs-discrete-distributions/
- https://medium.com/mytake/understanding-different-types-of-distributions-you-will-encounter-as-a-data-scientist-27ea4c375eec

Normal Distribution

- https://numpy.org/doc/stable/reference/random/generated/numpy.random.normal.html
- Wikipedia, “Normal distribution”, https://en.wikipedia.org/wiki/Normal_distribution
- https://www.w3schools.com/python/numpy_random_distribution.asp
- https://wtmatter.com/numpy-normal-distribution/
- https://www.kaggle.com/hamelg/python-for-data-22-probability-distributions

Uniform Distribution

- https://en.wikipedia.org/wiki/Continuous_uniform_distribution
- https://www.w3schools.com/python/numpy_random_uniform.asp
- https://numpy.org/doc/stable/reference/random/generated/numpy.random.Generator.uniform.html#numpy.random.Generator.uniform
- https://mathworld.wolfram.com/UniformDistribution.html

Logistic Distribution


- https://en.wikipedia.org/wiki/Logistic_distribution
- https://numpy.org/doc/stable/reference/random/generated/numpy.random.Generator.logistic.html#numpy.random.Generator.logistic
- https://www.w3schools.com/python/numpy_random_logistic.asp Weisstein, Eric W. “Logistic Distribution.” From MathWorld–A Wolfram Web Resource. http://mathworld.wolfram.com/LogisticDistribution.html
- Wikipedia, “Logistic-distribution”, http://en.wikipedia.org/wiki/Logistic-distribution
- https://wtmatter.com/numpy-logistic-distribution/

Binomial Distribution


https://numpy.org/doc/stable/reference/random/generated/numpy.random.Generator.binomial.html#numpy.random.Generator.binomial
https://en.wikipedia.org/wiki/Binomial_distribution
https://www.w3schools.com/python/numpy_random_binomial.asp
https://www.statisticshowto.com/probability-and-statistics/binomial-theorem/binomial-distribution-formula/


###### Use of seeds in generating pseudorandom numbers


- https://www.pcg-random.org/
- https://www.cs.hmc.edu/tr/hmc-cs-2014-0905.pdf
- https://www.pcg-random.org/
- https://stackoverflow.com/questions/63081108/how-can-i-store-and-restore-random-state-in-numpy-random-generator-instances
- https://numpy.org/doc/stable/reference/random/bit_generators/pcg64.htm
- https://www.sharpsightlabs.com/blog/numpy-random-seed/
- https://en.wikipedia.org/wiki/Random_seed
- https://www.researchgate.net/post/Can_someone_explain_what_is_seed_in_generating_a_random_number

###### Other - Markup etc

https://sebastianraschka.com/Articles/2014_ipython_internal_links.html


####  My Inital Project and Assignment Plan

- Jupyter Notebook created named - explaining.numpy.random
- Explain purpose of the package 
- Use the reamde file to give an overview of the package and withing Jupyter i will dig deeper into how to load numpy and some examples of using the subpackage.
- I intend to use this section to expalin more about the newest version of of numpy and the main changes. I will give an overview of the main chalenges software developers face when packages and APIs are upadted with examples
- Explain the use of the "simple random data" and "Permutations" functions.
- Within the readme i will exmplain the uses and withing the jupyter file will dig deeper with examples and sample code.
- Explain the use and purpose of at least five "Distribution" fucntions
- Use the README to give a brief desciption of each of the selected distibutions, i will use jupyter to code exmaples of how each can be used. I will generate random data using numpy and i will graph my results for visual representation.
- Explain the use of seeds in generating pseudorandom numbers 
- Withing the readme file give an overvie of seeds, why they are important, there usess and withing the Jupyter notebook give examples of how they are used, im going to review and reshearch how the PCG64 method outperforms the mersenne twister pseudo random number monthod from the previous version of Numpy
- Use markdown to add images and links within the jupyter notebook as referenced in assignment plan


## THE END