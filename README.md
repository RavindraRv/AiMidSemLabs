# AiMidSemLabs

Lab Assignment - 1

Learning Objective: To design a graph search agent and understand the use of a hash table, queue in state space search.

Reference: 
[1] Artificial Intelligence: a Modern Approach, Russell and Norvig (Fourth edition)
Chapter 2 and 3
[2] A first course in Artificial Intelligence, Deepak Khemani
Chapter 2

Problem Statement:

Write a pseudocode for a graph search agent. Represent the agent in the form of a flow chart. Clearly mention all the implementation details with reasons.
Write a collection of functions imitating the environment for Puzzle-8. 
Describe what is Iterative Deepening Search.
Considering the cost associated with every move to be the same (uniform cost), write a function which can backtrack and produce the path taken to reach the goal state from the source/ initial state.
Generate Puzzle-8 instances with the goal state at depth “d”.
Prepare a table indicating the memory and time requirements to solve Puzzle-8 instances (depth “d”) using your graph search agent.







Lab Assignment 4

Learning Objective: 
Game Playing Agent | Minimax | Alpha-Beta Pruning

Systematic adversarial search can lead to savings in terms of pruning of sub-trees resulting in lesser node evaluations

References:
[1] A first course in Artificial Intelligence, Deepak Khemani (Chapter 8)
[2] Artificial Intelligence: a Modern Approach, Russell and Norvig (Fourth edition)
(Chapter 5)

Problem:

What is the size of the game tree for Noughts and Crosses? Sketch the game tree.
Read about the game of Nim (a player left with no move losing the game). For the initial configuration of the game with three piles of objects as shown in Figure, show that regardless of the strategy of player-1, player-2 will always win. Try to explain the reason with the MINIMAX value backup argument on the game tree.
Implement MINIMAX and alpha-beta pruning agents. Report on number of evaluated nodes for Noughts and Crosses game tree.
Use recurrence to show that under perfect ordering of leaf nodes, the alpha-beta pruning time complexity is O(bm/2), where b is the effective branching factor and m is the depth of the tree.





Lab Assignment 5

Learning Objective:
Understand the graphical models for inference under uncertainty, build Bayesian Network in R, Learn the structure and CPTs from Data, naive Bayes classification with dependency between features.  

Reference:
https://www.bnlearn.com/
http://gauss.inf.um.es/umur/xjurponencias/talleres/J3.pdf

Problem Statement:
A table containing grades earned by students in respective courses is made available to you in (codes folder) 2020_bn_nb_data.txt. 
Consider grades earned in each of the courses as random variables and learn the dependencies between courses. 
Using the data, learn the CPTs for each course node.
What grade will a student get in PH100 if he earns DD in EC100, CC in IT101 and CD in MA101.
The last column in the data file indicates whether a student qualifies for an internship program or not. From the given data, take 70 percent data for training and build a naive Bayes classifier (considering that the grades earned in different courses are independent of each other) which takes in the student’s performance and returns the qualification status with a probability. Test your classifier on the remaining 30 percent data. Repeat this experiment for 20 random selection of training and testing data. Report results about the accuracy of your classifier.
Repeat 4, considering that the grades earned in different courses may be dependent.



Lab Assignment 7

Learning Objective:
To model the low level image processing tasks in the framework of Markov Random Field and Conditional Random Field. To understand the working of Hopfield network and use it for solving some interesting combinatorial problems


Reference:
http://www.cs.utoronto.ca/~strider/Denoise/Benchmark/
Interesting way to denoise an image using random walk: http://www.cs.toronto.edu/~fleet/research/Papers/BMVC_denoise.pdf
MRF Image Denoising: 
https://web.cs.hacettepe.edu.tr/~erkut/bil717.s12/w11a-mrf.pdf
Single Neuron and Hopfield Network: Chapter 40, 41, 42
Information Theory, Inference and Learning Algorithms, David MacKay
http://www.inference.phy.cam.ac.uk/mackay/itila/


Problem Statement:
Many low level vision and image processing problems are posed as minimization of energy function defined over a rectangular grid of pixels. We have seen one such problem, image segmentation, in class. The objective of image denoising is to recover an original image from a given noisy image, sometimes with missing pixels also. MRF models denoising as a probabilistic inference task. Since we are conditioning the original pixel intensities with respect to the observed noisy pixel intensities, it usually is referred to as a conditional Markov random field.  Refer to (3) above. It describes the energy function based on data and prior (smoothness). Use quadratic potentials for both singleton and pairwise potentials. Assume that there are no missing pixels. Cameraman is a standard test image for benchmarking denoising algorithms. Add varying amounts of Gaussian noise to the image for testing the MRF based denoising approach. Since the energy function is quadratic, it is possible to find the minima by simple gradient descent. If the image size is small (100x100) you may use any iterative method for solving the system of linear equations that you arrive at  by equating the gradient to zero. Extra Credit Challenge: Implement and compare MRF denoising with Stochastic denoising (reference 2).
For the sample code hopfield.m supplied in the lab-work folder, find out the amount of error (in bits) tolerable for each of the stored patterns.
Solve a TSP (traveling salesman problem) of 10 cities with a Hopfield network.  How many weights do you need for the network?  

