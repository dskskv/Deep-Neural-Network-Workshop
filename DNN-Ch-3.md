1) a better choice of cost function, known as the cross-entropy / regularization" methods
1) Which is a better choice of cost function from cross-entropy / regularization ?
2) How can we address the learning slowdown ? 
3) Who cares how fast the neuron learns, when our choice of learning rate was arbitrary to begin with?!
4) When should we use the cross-entropy instead of the quadratic cost?  
5) What do you mean by Epoch why not iteration ?
6) The cross-entropy is easy to implement as part of a program which learns using gradient descent and backpropagation
 That's quite a handy improvement by replacing cross-entropy with quadratic cost.
 But the interpretation of such improvements is always problematic ?
7) If regularization techniques, which gives much bigger improvements. So why so much focus on cross-entropy?
8) What does the cross-entropy mean? Is there some intuitive way of thinking about the cross-entropy? And how could we have dreamed up the cross-entropy in the first place?
Let's begin with the last of these questions: what could have motivated us to think up the cross-entropy in the first place? 
- What about the intuitive meaning of the cross-entropy? How should we think about it?
- How softmax layers of neurons better than cross-entropy ?
- why we're using the validation_data rather than the test_data to set good hyper-parameters?
- What is magic behind Validation Data with Train Data, Test Data ? How it help us to learn good hyper parameters ?

	