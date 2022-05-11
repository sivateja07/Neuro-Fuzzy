# Neuro Fuzzy
Hebbian Learning Rule, also known as Hebb Learning Rule, was proposed by Donald O Hebb. It is one of the first and also easiest learning rules in the neural network. It is used for pattern classification. It is a single layer neural network, i.e. it has one input layer and one output layer. The input layer can have many units, say n. The output layer only has one unit. Hebbian rule works by updating the weights between neurons in the neural network for each training sample.

## Hebbian Learning Rule Algorithm : 

1)Set all weights to zero, wi = 0 for i=1 to n, and bias to zero.

2)For each input vector, S(input vector) : t(target output pair), repeat steps 3-5.

3)Set activations for input units with the input vector Xi = Si for i = 1 to n.

4)Set the corresponding output value to the output neuron, i.e. y = t.

5)Update weight and bias by applying Hebb rule for all i = 1 to n


## Perceptron Algorithm

The Perceptron is inspired by the information processing of a single neural cell called a neuron.

A neuron accepts input signals via its dendrites, which pass the electrical signal down to the cell body.

In a similar way, the Perceptron receives input signals from examples of training data that we weight and combined in a linear equation called the activation.

## activation = sum(weight_i * x_i) + bias
The activation is then transformed into an output value or prediction using a transfer function, such as the step transfer function.

## prediction = 1.0 if activation >= 0.0 else 0.0
In this way, the Perceptron is a classification algorithm for problems with two classes (0 and 1) where a linear equation (like or hyperplane) can be used to separate the two classes.

It is closely related to linear regression and logistic regression that make predictions in a similar way (e.g. a weighted sum of inputs).

The weights of the Perceptron algorithm must be estimated from your training data using stochastic gradient descent.


## MADALINE


A multilayer network of ADALINE units is known as a MADALINE.

• MADALINE is a three-layer (input, hidden, output), fully connected, feed-forward artificial neural network architecture for classification that uses
ADALINE units in its hidden and output layers, i.e. its activation function is the sign function.

• Three different training algorithms for MADALINE networks, which cannot be learned using backpropagation because the sign function is not
differentiable, have been suggested, called Rule I, Rule II and Rule III.

• MADALINE Rule 1 (MRI) - The first of these dates back to 1962 and cannot adapt the weights of the hidden-output connection.[10]

• MADALINE Rule 2 (MRII) - The second training algorithm improved on Rule I and was described in 1988.[8] The Rule II training algorithm is based on a
principle called "minimal disturbance". It proceeds by looping over training examples, then for each example, it:

• finds the hidden layer unit (ADALINE classifier) with the lowest confidence in its prediction,


• tentatively flips the sign of the unit,

• accepts or rejects the change based on whether the network's error is reduced,

• stops when the error is zero.

• MADALINE Rule 3 - The third "Rule" applied to a modified network with sigmoid activations instead of signum; it was later found to be equivalent to
backpropagation.[10]

• Additionally, when flipping single units' signs does not drive the error to zero for a particular example, the training algorithm starts flipping pairs of
units' signs, then triples of units, etc.[8]
