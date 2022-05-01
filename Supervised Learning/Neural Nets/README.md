# Neural Nets


## What is neural nets?

Artificial neural networks (ANNs), usually simply called neural networks (NNs), are computing systems inspired by the biological neural networks that constitute animal brains.

An ANN is based on a collection of connected units or nodes called artificial neurons, which loosely model the neurons in a biological brain. Each connection, like the synapses in a biological brain, can transmit a signal to other neurons. An artificial neuron receives a signal then processes it and can signal neurons connected to it. The "signal" at a connection is a real number, and the output of each neuron is computed by some non-linear function of the sum of its inputs. The connections are called edges. Neurons and edges typically have a weight that adjusts as learning proceeds. The weight increases or decreases the strength of the signal at a connection. Neurons may have a threshold such that a signal is sent only if the aggregate signal crosses that threshold. Typically, neurons are aggregated into layers. Different layers may perform different transformations on their inputs. Signals travel from the first layer (the input layer), to the last layer (the output layer), possibly after traversing the layers multiple times.


## How do neural nets works?

A simple neural network includes an input layer, an output (or target) layer and, in between, a hidden layer. The layers are connected via nodes, and these connections form a “network” – the neural network – of interconnected nodes.

A node is patterned after a neuron in a human brain. Similar in behavior to neurons, nodes are activated when there is sufficient stimuli or input. This activation spreads throughout the network, creating a response to the stimuli (output). The connections between these artificial neurons act as simple synapses, enabling signals to be transmitted from one to another. Signals across layers as they travel from the first input to the last output layer – and get processed along the way.

When posed with a request or problem to solve, the neurons run mathematical calculations to figure out if there’s enough information to pass on the information to the next neuron. Put more simply, they read all the data and figure out where the strongest relationships exist. In the simplest type of network, data inputs received are added up, and if the sum is more than a certain threshold value, the neuron “fires” and activates the neurons it’s connected to.

As the number of hidden layers within a neural network increases, deep neural networks are formed. Deep learning architectures take simple neural networks to the next level. Using these layers, data scientists can build their own deep learning networks that enable machine learning, which can train a computer to accurately emulate human tasks, such as recognizing speech, identifying images or making predictions. Equally important, the computer can learn on its own by recognizing patterns in many layers of processing.

So let’s put this definition into action. Data is fed into a neural network through the input layer, which communicates to hidden layers. Processing takes place in the hidden layers through a system of weighted connections. Nodes in the hidden layer then combine data from the input layer with a set of coefficients and assigns appropriate weights to inputs. These input-weight products are then summed up. The sum is passed through a node’s activation function, which determines the extent that a signal must progress further through the network to affect the final output. Finally, the hidden layers link to the output layer – where the outputs are retrieved.

## Datasets

### Description:

Fashion-MNIST is a dataset of Zalando's article images consisting of a training set of 60,000 examples and a test set of 10,000 examples. Each example is a 28x28 grayscale image, associated with a label from 10 classes.

### Homepage: https://github.com/zalandoresearch/fashion-mnist

### Source code: tfds.image_classification.FashionMNIST

### Versions:

3.0.1 (default): No release notes.
### Download size: 29.45 MiB

### Dataset size: 36.42 MiB

### Auto-cached (documentation): Yes

### Figures:

![image](https://user-images.githubusercontent.com/98139045/166153435-98b4fbb9-a9b0-478c-88c2-1eea7094580d.png)


## References

https://www.sas.com/en_us/insights/analytics/neural-networks.html#:~:text=How%20Neural%20Networks%20Work,neuron%20in%20a%20human%20brain.
https://en.wikipedia.org/wiki/Artificial_neural_network
