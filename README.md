
# Programming for Data Analysis Assignment - Semester 2

## Brendan Ryan, GMIT Student


### Details of Git Repository

The repository for the assigment and all the files are located here https://github.com/brendantipp/sem2_prog_data_analysis_assignment

### Assignment Details and the Tasks for this assignment 

1. Explain the overall purpose of teh numpy.random package
2. Explain the use of the "simple random data" and "Permutations" functions
3. Explain the use and purpose of at least five "Distribution" fucntions
4. Explain the use of seeds in generating pseudorandom numbers

Please note: My initial project plan for this assigment along with references and research links used can be found at the end of this README


### How to run the Jupyter Notebook

To run the notebook dowload from the repository to your local hard drive and open with Jupyter Notebooks - www.jupyter.org


## Purpose of the Numpy Library and why is it so widely used

NumPy is a pyton library used for working with arrays, it was created in 2005 by Travis Oliphant. It is an open source project and you can use if freely, NumPy stands for Numerical Python.

NumPy is the fundamental package for scientific computing in Python. It is a Python library that provides a multidimensional array object, various derived objects (such as masked arrays and matrices), and an assortment of routines for fast operations on arrays, including mathematical, logical, shape manipulation, sorting, selecting, I/O, discrete Fourier transforms, basic linear algebra, basic statistical operations, random simulation and much more.

At the core of the NumPy package, is the ndarray object. This encapsulates n-dimensional arrays of homogeneous data types, with many operations being performed in compiled code for performance source - - source https://docs.scipy.org/doc/numpy-1.15.1/user/whatisnumpy.html

#### Why we use Numpy "its quick and efficient"
In python we have lists that server the purpose of arrays, however are slow to process - Numpy aims to provide an array object that is 50 times faster than traditional python lists and is more efficient !!! NumPy arrays are stored in one continous place in memory and Numpy lists are optimized to work with the latest CPU achitectures.

W3schools.com gives an nice easy explanation https://www.w3schools.com/python/numpy_intro.asp

    #we can import the numpy module as follows using np to give a shortened name to the package for ease of use
    import numpy as np



### Purpose of the Numpy.random subpackage


NumPy offers the random moudle to work with random numbers - random is a subpackage of Numpy and is available in the numpy library. The module contains the functions which are used for generarting random numbers. The module contains some simple random data generation methods, some premutation and distribution functions , and random generator functions.

There is a random() function built into python and you might ask why use the numpy.random package - I found the following explanation wording at https://stackoverflow.com/questions/7029993/differences-between-numpy-random-and-random-random-in-python benefical to a novice like me!

"The numpy.random library contains a few extra probability distributions commonly used in scientific research, as well as a couple of convenience functions for generating arrays of random data. The random.random library is a little more lightweight, and should be fine if you're not doing scientific research or other kinds of work in statistics" . So numpy.random wins our vote.

Within the numpy.random subpackage there are a number of functions and these can be broken down into 

- Simple Random Data functions
- Permutation funcitons
- Distribution functions
- Seed functions

More information on the above can be found in more detail at https://numpy.org/doc/stable/reference/random/

### Important changes made to the Numpy.random package and why these changes are important  to sofware developers

At the time of writing this assignment them most uptodate version of the Numpy module is v 1.19. It is important to note that the latest versions of the Numpy.random package contain updated functions.  In paticular there has been some major changes to the Simple Random Data functions - some of the old functons where almost duplicates of each other and were essentially the same function. The distributions and Permutation functions are very similar in both the new and older versions of the Numpy.random package

It is the job of a software developer to keep up to date with these changes and to maintain their code. In the case of the numpy.random library developers can find the most recent documentation available at https://numpy.org/doc/stable/




#### Simple random data functions

These functions allow us to define sequences and arryas of integers  random real values, choice to generate a random sample from a give 1 dimesional array and bytes to return radmom bytes. It is worth noting the simple random data functions have been revised and condensed in the newer version of the numpy.random package.

The following are the Simple random data fucntions

- integer()
- random()
- choice()
- bytes

In my Jupyter notebook I go through each of the above with example, for the choice funciton i give an exmaple of this fucntion can be used to generate six random numbers for a lottery.


#### Permutations 

There are two permuation functions that are available to us and these provide for random shuffling of data 

- shuffle()
- permuation()

Shuffle function - modifies a sequence in place by shuffing its contents 
permutation function - always returns a shuffed version of the original sequence

In my Jupyter notebook I go through each of the two examples to test how they work in more detail. 


## Distribution Functions 


To be completed 


## Explaining the use of Seeds in generating Pseudorandm Numbers

There’s a fundamental problem when using computers to simulate or work with random processes. 
That is computers are completely deterministic, not random.
Setting aside some rare exceptions, computers are deterministic by their very design. So if you give a computer a certain input, it will precisely follow instructions to produce an output.
If the input is the same, then the output will be the same. - THAT’S HOW COMPUTERS WORK.
Therefor it’s very difficult to create truly “random” numbers on a computer. Computers get around this by using pseudo-random number generators
Pseudo-random numbers are computer generated numbers that appear random, but are actually predetermined
We use np.random.seed when we need to generate random numbers or mimic random processes in NumPy.
In order to work properly, pseudo-random number generators require a starting input. We call this starting input a “seed.”.
In my jupyter notebook I go through the following examples - TBC


tO BE COMPLETED add items from testing in jupyter noteook



## Lessons learned and conclusions


#### Project Plan

Jupyter Notebook created named - explaining.numpy.random

My Assignment Plan 

Explain purpose package 

Use the reamde file to give an overview of the package and withing Jupyter i will dig deeper into how to load numpy and some examples of using the subpackage.

I intend to use this section to expalin more about the newest version of of numpy and the main changes. I will give an overview of the main chalenges software developers face when packages and APIs are upadted with examples 

Explain the use of the "simple random data" and "Permutations" functions

Within the readme i will exmplain the uses and withing the jupyter file will dig deeper with examples and sample code 

Explain the use and purpose of at least five "Distribution" fucntions

Use the reamde to give a brief desciption of each of the selected distibutions, i will use jupyter to code exmaples of how each can be used. I will genrate random data using numpy and i will graph my restults for visual representation.

Explain the use of seeds in generating pseudorandom numbers
 
Withing the readme file give an overvie of seeds, why they are important, there usess and withing the Jupyter notebook give examples of how they are used, im going to review and reshearch how the PCG64 method outperforms the mersenne twister pseudo random number monthod from the previous version of Numpy


References used and research undertaken


Understanding Numpy
https://stackoverflow.com/questions/7029993/differences-between-numpy-random-and-random-random-in-python


https://numpy.org/doc/stable/reference/random/generator.html#numpy.random.Generator
https://numpy.org/doc/stable/reference/random/index.html
https://docs.scipy.org/doc/numpy-1.15.1/reference/routines.random.html













