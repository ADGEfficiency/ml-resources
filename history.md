## Sources

[2019 - Yan LeCun - ISCC]()

## History of deep learning

Hardware is important!

### 1943 

[McGulloch-Pitts Binary Neuron](https://en.wikipedia.org/wiki/Artificial_neuron#History) - the Linear Threshold Unit

Used a threshold as the non-linearity (similar to logistic regression)

Binary inputs & outputs only

### 1958

[Perceptron](https://en.wikipedia.org/wiki/Perceptron) - Frank Rosenblatt

>	the embryo of an electronic computer that [the Navy] expects will be able to walk, talk, see, write, reproduce itself and be conscious of its existence - New York Times, 1958

### 1960

[Adaptive Linear Neuron - ADALINE](https://en.wikipedia.org/wiki/ADALINE) - Bernard Widrow

Introduced the bias

### 1969 - 1982

Neural net winter
- using the wrong neuron (binary)
- prevented thinking about gradient based methods for multilayer networks

### 1982

[Hopfield nets](https://en.wikipedia.org/wiki/Hopfield_network) - John Hopfield
- fully-connected recurrent binary networks
- memory

### 1985

[Boltzmann Machines](https://en.wikipedia.org/wiki/Boltzmann_machine) - Geoffrey Hinton
- binary stochastic networks with hidden units
- stochastic, generative counterpart of Hopfield networks

### 1985

[Backpropagation](https://en.wikipedia.org/wiki/Backpropagation#History) - Rumelhart, Hinton and Williams
- because of the sigmoid - enabled by fast floating points on Sun Workstations

### 1987

Modern form of backprop - Yann LeCun's PhD

### 1989

Convolution - Yan LeCun
- Inspired by [Hubel & Wiesel 1962] & [Fukushima 1982] (Neocognitron)
- simple cells detect local features
- complex cells “pool” the outputs of simple cells within a retinotopic neighborhood.

### 1992

LeNet
- character recognition

### 1995

AT&T check reader

### 1997

LSTMs

### 1995 - 2006

Second neural network winter
- slow hardware
- data scarce
- tools built from scratch - no open source
- tools shape research directions

### 2013

AlexNet

### 2014

GoogLeNet

### 2015

ResNet
- ResNet 50 & 100 = used in production
- each photo uploaded to Facebook goes through a handful of cov nets within two seconds
