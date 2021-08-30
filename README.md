# MultiLayerPreceptronPyTorch-MNIST
  
Building a simple multilayer perceptron model in PyTorch to do handwritten digit classification.
This is done very similary to the logistic regression example, but instead of going straight to a 10-d vector representing our output predictions, we might first transform to a 500-d vector with a "hidden" layer, then to the output of dimension 10.

![MLP](https://user-images.githubusercontent.com/66415170/131272072-63579e91-306c-460c-b291-f32a4740547f.png)

One more important thing to consider is that We typically include nonlinearities between layers of a neural network. There's a number of reasons to do so. For one, without anything nonlinear between them, successive linear transforms (fully connected layers) collapse into a single linear transform, which means the model isn't any more expressive than a single layer. On the other hand, intermediate nonlinearities prevent this collapse, allowing neural networks to approximate more complex functions.

### MNIST Dataset
The MNIST dataset is very popular machine learning dataset, consisting of 70000 grayscale images of handwritten digits, of dimensions 28x28.

<img width="352" alt="mnist" src="https://user-images.githubusercontent.com/66415170/131272210-d5b0623f-6279-42b5-a877-022a3959d526.png">

We split the dataset into two separate groups:

Number of MNIST training examples: 60000

Number of MNIST test examples: 10000

### Goal
So, the goal is to predict which digit is in each image in the testing set. Then, we compute an accuracy by seeing how many we got correct!

###### Introduction to Machine Learning - Duke University - Coursera

