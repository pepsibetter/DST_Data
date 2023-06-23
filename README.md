## Introduction
This repository stores data and code of using deep learning methods for solving Directed Steiner Tree problems, and the data are all included in JSON files.

## Data description
The title of each file denotes graph type and scale, such as "PL_100" representing a power law graph and scale of 100 (i.e., 100 nodes). Each file consists of weights, adjacency lists, problem instances, optimal solutions to problem instances via a DP algorithm, the probabilities of nodes whether they belong to optimal solutions given by the deep learning model, and the deep learning solutions to problem instances. Usually, the first 70% of instances are used as training data, while the rest 30% as testing data.

## Training tricks
In fact, the training procedure is really sensitive to the (edge) structure of the graphs. We recommend using incremental training, i.e., training from a small-scale graph to a large-scale graph, but only for those structure that do not change a lot, such as power law graphs. Otherwise, this training strategy may not be suitable. 

## Updates
The updates of data will be announced later as the space here is limited.
