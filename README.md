# DeepSimpsonsGen
An attempt to generate new faces for Simpsons characters using DCGANS

## Lets start with GANS:

![](https://github.com/smaranjitghose/DeepSimpsonsGen/blob/master/assets/gans_1.png)

#### Generator
The Generator takes random noise as an input and generates samples as an output. It’s goal is to generate such samples that will fool the Discriminator to think that it is seeing real images while actually seeing fakes. We can think of the Generator as a counterfeit.

#### Discriminator
Discriminator takes both real images from the input dataset and fake images from the Generator and outputs a verdict whether a given image is legit or not. We can think of the Discriminator as a policeman trying to catch the bad guys while letting the good guys free.

![](https://github.com/smaranjitghose/DeepSimpsonsGen/blob/master/assets/gans_2.png)

#### Minimax Representation
If we think once again about Discriminator’s and Generator’s goals, we can see that they are opposing each other. Discriminator’s success is a Generator’s failure and vice-versa. That is why we can represent GANs framework more like Minimax game framework rather than an optimization problem.



