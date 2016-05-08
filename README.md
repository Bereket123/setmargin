Preference Elicitation via Set-wise Max-margin
==============================================

Implementation of the set-wise max-margin (setmargin for short) preference
elicitation algorithm.

For details, see the paper:

<a href="https://arxiv.org/abs/1604.06020" target="_blank">Stefano Teso, Andrea Passerini, Paolo Viappiani. Constructive Preference Elicitation by Setwise Max-margin Learning. proceedings of 25th International Joint Conference on Artificial Intelligence. 2016. (To appear)</a>

## Requirements

This package requires the following packages:

- [numpy](http://www.numpy.org/)
- [gurobi](http://www.gurobi.com/)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/)

## Usage

To run the IJCAI-16 experiments, simply type:
```
    python ijcai16.py run-synthetic
    python ijcai16.py run-pc-with-costs
```
To perform preference elicitation on a specific dataset with given parameters,
type:
```
    python ijcai16.py run $dataset $parameters
```
For instance, to run 20 trials of length 10 with set size 3 on the synthetic
dataset, write:
```
    python ijcai16.py run synthetic -T 20 -n 10 -k 3
```
See:
```
    python ijcai16.py --help
```
for a full list of the accepted arguments.

## Funding

The project is supported by the CARITRO Foundation through grant E62I15000530007.
