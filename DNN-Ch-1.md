- Neural Networks and Deep Learning
- How DNN may be applied to other problems in computer vision, and also in speech, natural language processing, and other domains
- perceptron - inspired by earlier work by Warren McCulloch and Walter Pitts.
- Modern NN- sigmoid neuron. 
- how do perceptrons work?
- ex. NAND gates are universal for computation, it follows that perceptrons are also universal for computation.
- The computational universality of perceptrons is simultaneously reassuring and disappointing. It's reassuring because it tells us that networks of perceptrons can be as powerful as any other computing device. But it's also disappointing, because it makes it seem as though perceptrons are merely a new type of NAND gate. That's hardly big news!
- Neural networks can simply learn to solve problems, sometimes problems where it would be extremely difficult to directly design a conventional circuit.
- Why Sigmoid Neuron network people uses instead of Perceptron ?
- How should we interpret the output from a sigmoid neuron ?
- Multilayer perceptrons or MLPs 
- feedforward neural networks vs Recurrent Neural Networks
- How to use correct input neuron, output neuron, number of hidden layers based on problem statement !
- Is there some heuristic that would tell us in advance that we should use the N-output encoding instead of the N-output encoding?
- Now no assumption , We want fact ! It does this by weighing up evidence from the hidden layer of neurons. What are those hidden neurons doing ?
- Importance of vector
- Math behind Neural Network Learning
- How it is easy to program Algebraic form of Sigmoid or any other NN Fn ?
- How to minimize the Cost C(w,b) weights and biases with Gradient Descent. The way gradient descent works ? variations of gradient descent ?
- How to develop good neural network architecture ! How to tune hyper-parameters such as learning rate, hidden layers ?
- Why introduce the quadratic cost? 
- Using calculus to minimize that just won't work!
- Okay, so calculus doesn't work. Fortunately, there is a beautiful analogy which suggests an algorithm which works pretty well. 
- How stochastic gradient descent can be used to speed up learning ?
- What is incremental learning ? incremental learning vs stochastic gradient descent
- 


handwriting recognition

changing the weights and biases over and over to produce better and better output. The network would be learning.



Sigmoid neurons are similar to perceptrons, but modified so that small changes in their weights and bias cause only a small change in their output. That's the crucial fact which will allow a network of sigmoid neurons to learn.

At first sight, sigmoid neurons appear very different to perceptrons. The algebraic form of the sigmoid function may seem opaque and forbidding if you're not already familiar with it. In fact, there are many similarities between perceptrons and sigmoid neurons, and the algebraic form of the sigmoid function turns out to be more of a technical detail than a true barrier to understanding.

How should we interpret the output from a sigmoid neuron? Obviously, one big difference between perceptrons and sigmoid neurons is that sigmoid neurons don't just output 0 or 1. They can have as output any real number between 0 and 1, so values such as 0.173… and 0.689… are legitimate outputs. This can be useful, for example, if we want to use the output value to represent the average intensity of the pixels in an image input to a neural network. But sometimes it can be a nuisance. Suppose we want the output from the network to indicate either "the input image is a 9" or "the input image is not a 9". Obviously, it'd be easiest to do this if the output was a 0 or a 1, as in a perceptron. But in practice we can set up a convention to deal with this, for example, by deciding to interpret any output of at least 0.50.5 as indicating a "9", and any output less than 0.50.5 as indicating "not a 9".

Excersize





And it's possible that recurrent networks can solve important problems which can only be solved with great difficulty by feedforward networks.






Why I would use hidden layers ? we could legitimately get a answer in many other ways (say, through translations of the above images, or slight distortions). But it seems safe to say that at least in this case we'd conclude that the input was a 0.


Nothing says that the n-layer neural network has to operate in the way first I described, with the hidden neurons detecting simple component shapes. Maybe a clever learning algorithm will find some assignment of weights that lets us use only 4 output neurons. But as a heuristic the way of thinking I've described works pretty well, and can save you a lot of time in designing good neural network architectures.

More hidden layers it doesn't mean more accurate answer ! Maybe a clever learning algorithm will find some assignment of weight that lets us use very less number of output neurons. But as a heuristic the way of thinking it has been described and works pretty well. 
P.S Always Design good neural network architecture ! tune hyper-parameters such as learning rate, hidden layers ?


How to minimize the Cost C(w,b) weights and biases with Gradient Descent. The way gradient descent works ? variations of gradient descent ?Cons: it turns out to be necessary to compute second partial derivatives of Cost fn, and this can be quite costly ? 

To see why it's costly, suppose we want to compute all the second partial derivatives ∂2C/∂vj∂vk∂2C/∂vj∂vk. If there are a million such vjvj variables then we'd need to compute something like a trillion (i.e., a million squared) second partial derivatives. That's going to be computationally costly ! Any Alternative ! Yes always "active area of investigation"

Why introduce the quadratic cost? 

Using calculus to minimize that just won't work!

Okay, so calculus doesn't work. Fortunately, there is a beautiful analogy which suggests an algorithm which works pretty well. 

How stochastic gradient descent can be used to speed up learning ?

What is incremental learning ? incremental learning vs stochastic gradient descent

Some people get hung up thinking: "Hey, I have to be able to visualize all these extra dimensions". And they may start to worry: "I can't think in four dimensions, let alone five (or five million)". Is there some special ability they're missing, some ability that "real" supermathematicians have? Of course, the answer is no. Even most professional mathematicians can't visualize four dimensions especially well, if at all. The trick they use, instead, is to develop other ways of representing what's going on. That's exactly what we did above: we used an algebraic (rather than visual) representation of ΔCΔC to figure out how to move so as to decrease C. 



sophisticated algorithm ≤≤ simple learning algorithm + good training data.

While our neural network gives impressive performance, that performance is somewhat mysterious. The weights and biases in the network were discovered automatically. And that means we don't immediately have an explanation of how the network does what it does.

