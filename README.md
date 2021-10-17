# Simple-Neural-Network-code
In this code you will learn simply how to crate Neural Network. Before that how does Neural network learn?

How does a neural network learn ?

Creating variables and making them interact with each other is great, but that is not enough to make the whole neural network learn by itself. We need to prepare a lot of data to give to our network. Those data include the inputs and the output expected from the neural network.

First of all, remember that when an input is given to the neural network, it returns an output. On the first try, it can’t get the right output by its own (except with luck) and that is why, during the learning phase, every inputs come with its label, explaining what output the neural network should have guessed. If the choice is the good one, actual parameters are kept and the next input is given. However, if the obtained output doesn’t match the label, weights are changed. Those are the only variables that can be changed during the learning phase. This process may be imagined as multiple buttons, that are turned into different possibilities every times an input isn’t guessed correctly.

To determine which weight is better to modify, a particular process, called “backpropagation” is done. We won’t linger too much on that, since the neural network we will build doesn’t use this exact process, but it consists on going back on the neural network and inspect every connection to check how the output would behave according to a change on the weight.
Finally, there is a last parameter to know to be able to control the way the neural network learns : the “learning rate”. The name says it all, this new value determines on what speed the neural network will learn, or more specifically how it will modify a weight, little by little or by bigger steps. 1 is generally a good value for that parameter.
Perceptron

So, we know the basics, let’s check about the neural network we will create. The one explained here is called a Perceptron and is the first neural network ever created. It consists on 2 neurons in the inputs column and 1 neuron in the output column. This configuration allows to create a simple classifier to distinguish 2 groups. 

In the code when you insert 1 and 0, If you replace the “true”s by 1 and the “false”s by 0 and put the 4 possibilities as points with coordinates on a plan, then you realize the two final groups “false” and “true” may be separated by a single line. This is what a Perceptron can do.

On the other hand, if we check the case of the “exclusive or” (in which the case “true or true” (the point (1,1)) is false), then we can see that a simple line cannot separate the two groups, and a Perceptron isn’t able to deal with this problem.
So, the Perceptron is indeed not a very efficient neural network, but it is simple to create and may still be useful as a classifier.

Thank you!
