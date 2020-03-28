This is not an instruction file nor a howto, just a memo explaining few thing  

### Activation function
Here are the four most used activation function  

![function](./4function.png)

### Perceptron algorithm
Let's build a basic warning system based in AND logic  
We have two sensors, here are the rules that trigger the warning
* If both or one of them is disabled, the warning is trigged
* If both are enabled, the warning is not trigged

To encode the problem, inputs are represented as follows.
> 0 means disabled,  
1 means enabled.  
Output is represented as follows.  
0 means enabled,  
1 means disabled. 

*The following table summarizes this*

| Sample | Sensor 1 | Sensor 2 | Alarm |
|:---:|:---:|:---:|:---:|
| 1 | 0 | 0 | 0 |
| 2 | 0 | 1 | 0 |
| 3 | 1 | 0 | 0 |
| 4 | 1 | 1 | 1 |
***

First, an **object** of the NeuralNet class is **created**.  
After that, this object is used to **initialize the neural net** with two neurons in the input layer,  
none in the hiddenlayer, and one neuron in the output layer.  
Then, a message and the untrained neural net are shown on the screen.  
Another object of the NeuralNet class is created and represents the trained neural net.  
After that, the **testNet object is set** with the training input dataset (the first column has bias values),  
training output dataset, maximum number of epochs, target error, learning rate, training type (perceptron),  
and activation function (step).  
Then, the trainNet method is called to **train the neural net**.  
To finalize, the perceptron-trained net results are printed.  

**Note:** The neurons are initialized with pseudo-random values, each time this
code is run, the results change.

 

- [x] Perceptron
- [ ] Adaline algorithm comment
- [ ] NEAT


## Sources
- Maths comprehension with [hugolgst](https://github.com/hugolgst/the-math-behind-an-artificial-neural-network)  
- General [knowledge](http://neuralnetworksanddeeplearning.com/)
