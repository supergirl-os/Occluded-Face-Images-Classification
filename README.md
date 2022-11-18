# Occluded Face Images Classification
Classification of Occluded Face Images Based on Sparse Representation based Classifier (SRC) [1] and Voting Mechanism

1. Check the data characteristics in the dataset, and determine the image block size. The unoccluded face as the training data, and the occluded face as the test data.
2. Apply the SCR algorithm to build a dictionary and classify the testset based on block voting.
3. Use Orthogonal Matching Pursuit (OMP) to solve the optimization problem for sparse representation.

## Structure

```
-Occluded Face Images Classification
|---dataloader.py  # Load the SVHN dataset
|---main.py 		 
|---params.py       # Set param
|---utils.py
```

## Requirements

- Python 3.8
- numpy 3.9
- opencv 4.5
- pillow 8.1.2

## Reference

[1] Wright J, Yang A Y, Ganesh A, et al. Robust face recognition via sparse representation[J]. IEEE transactions on pattern analysis and machine intelligence, 2008, 31(2): 210-227.