# Synthetic-Data-Generation-with-CTGAN
Synthetic Data Generation with CTGAN
What are GANs?
GANs, or generative adversarial networks, are algorithms that use two neural networks competing against each other (thus the “adversarial”) in order to generate synthetic data [2]. The two neural networks are known as the generator and the discriminator.

The discriminator's goal is to be able to tell apart real and synthetic data. Meanwhile, the generator's goal is to create high quality synthetic data that fools the discriminator. 
The CTGAN Loss Function
How do these GANs improve over time? The key to training are the loss functions, a set of formulas that tell each network how to improve after each training iteration (or epoch). The discriminator and generator each have their own loss values. Epoch after epoch, these networks learn by trying to minimize their loss function.

Loss functions are an area of active research, and many approaches have been proposed for different uses. In CTGAN, we have formulated custom loss functions for the purposes of creating synthetic data.





The discriminator is learning to produce low values if the data is synthetic and high values if it is real. The range of these values is dependent on linear transformations and dimensions of the input data. [1]

Here is an example of generator and discriminator loss values from CTGAN, varying over 1000 epochs.
