---
type: note
---
04/02/2024 11:50

  #machine_learning

In a convolutional [[Neural Network]], the input data is first [[Convolution|Convolved]] with a filter (or kernel) to create a feature map. The process may be repeated on the resulting feature map and again on that result. This, along with pooling, makes up the feature learning process which allows the NN to recognize certain characteristic features in the data that allow it to distinguish and classify different parts of the data. Applied to images, the CNN may learn the shape of a leg, ear, or other body parts of a cat that allows it to recognize a cat due to the presence of its learned features. If features of dogs are learned also, it can learn to distinguish between cats and dogs.

To calculate the size of a resulting feature map:
$$
N=\frac{n+2p-f}{s}+1
$$
where
- $N$ = feature map width/height 
- $n$ = input width/height
- $p$ = padding
- $f$ = filter width/height
- $s$ = stride

The number of weights and biases for a certain layer:
$$
P=(d)(f)(f)(ch)+d
$$
where
- $d$ = filter depth
- $ch$ = number of channels in input

>[!note]
>These formulas are given for a square array of data and square filter such that the width and height are the same