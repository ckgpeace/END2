## Session1

### What is a neural network neuron?
Neurons are the units in neural network which consists the trasitory values for a given input. A DNN consists of many layers and each layer consists of many neurons and each neuron holds a specific value at one specific instance of an input. For the case of an image, neurons can be thought as pixels of the image and each layer of the DNN has many pixel which are resultant of processing of previous neurons and weights.

### What is the use of the learning rate?
Learning rate is the step size the optimizer takes in search of finding the minimum of the loss fucntion in each iteration. High LR values might help in finding the minimum faster but it can cause divergent behaviors. On the other hand very low LR values might lead to right minima of the loss function but it would require many updated to reach to the minima and makes the convergence slow.

![image](https://user-images.githubusercontent.com/16939617/121838422-6ba59680-ccf5-11eb-83e6-66058f6b3d5d.png)

### How are weights initialized?
Weight in a NN are initialized randomly usually. This the optimal way in comparison to initializing all weights to a fixed value as randomly initialized weights would require lower steps to reach the optimal weights as compared a fixed value initial weight. In layman terms, shifting(moving from initial value of weights to a final value after one iteration) of weights from a fixed value to some distirbution after first iteration is lower when the weights are initialized randomly. For instance, if we initialize with zero the weights won't update.

### What is "loss" in a neural network?
Loss is the translation of difference between the neural network prediction and the actual value. There are various loss function based on the dataset, the different loss funtions are Mean Squared error, Categorical Cross Entropy, Negative Log-Likelihood (NLL) etc.

The loss function example:

![image](https://user-images.githubusercontent.com/16939617/121840987-0ce31b80-ccfb-11eb-8748-df58ef632ce6.png)

### What is the "chain rule" in gradient flow?
The chain rule in gradient flow signifies that the gradients updation is linked process. The gradient update of one layer depends on the previous layer and so on. It also signifies that the updation can be deacreasing or increasing in the chain and care should be taken to avoid sitiations like vanishing gradient or exploding gradient problem. The back propagation helps after the optimizer step updates the gradients using chain rule of differential world.

![image](https://user-images.githubusercontent.com/16939617/121841589-423c3900-ccfc-11eb-9637-53d2f101e4da.png)





