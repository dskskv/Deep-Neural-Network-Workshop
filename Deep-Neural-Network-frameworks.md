## The Center of Data Science and Computer Vision, Department of Computer Science, University of Kachchh

This Article helps to choose appropriate Deep Neural Network framework according to use cases, following are the benchmarks with comparisions.

"A Neural Network is a Computational Graph"
***
There are following Deep neural network frameworks are Introduced by various research group and widely adopted by industries and researchers.

1. Caffe
2. CNTK
3. TensorFlow
4. Theano
5. Torch

*"Simplity of C in Lua and Complexity of C++ in Python"*
***

| Caffe         									| Torch7      																		|
| --------------------------------------------------|-----------------------------------------------------------------------------------|
| 1. It is Easy, limited use cases of CNNs. 		| 1. Torch7 is more transparent as compared to Theano.								|
| 2. Framework has written in C++ and having 		| 2. Originally written in C , wrapped with Lua.									|
|    convenience wrappers like Python.      	    | 3. Torch is build for Numeric Computations.										|
| 3. Each Node is Layer.							| 4. There is no compile time.														|
| 4. Main Strength: 								| 5. Excellent for Convolutional networks											|
|  	4.1. GPU Implementation							| 6. Worth Noting that Temporal Convolution can be done in Tensorflow / Theano via Conv2d but that's trick !|
|  	4.2. Model Representation						|    											|
| 5. Current Trends									| 7. Rich set of RNNs Available through a non official Extensions.					|
|  	5.1. Semantic Segmentation						| 8. There are multiple ways to define network 										|
|  	5.2. Funny CNN 									|	 - Stack of layers 																|
|  	5.3. Fast R-CNN 								|    - Graph of layers 																|
|  	5.4. Batch Normalization						|	 But essentially network is defined as a graph of layers.  						|
| 6. Layers are defined in C++, while networks are defined via Protobuf. 	| 9. Torch is sometimes considered less flexible because for new layers types and User have to Implement the full forward, backward & gradient input update. | 7. Caffe has PyCaffe client Interface & command line Interface, model has to defined in Protobuf.	| |
 		|	10. Defining new layer is much easier and the difference between new layers-definition & network definition is much minimal.									|
										| 11. Runs on LuaJIT so it is much faster than C++ / C# / Java.						|
| 8. Cross- Platform due to Core C++ Implementation.| 12. Who uses Torch:																|
|													|      - Google (Supporter), Deepmind works on Torch, started to do Codemigration 	|
|													|	   - Nvidia (with Cudnn)														|
|													|	   - Facebook (with Cudnn)														|
|													|      - Twitter (with Cudnn)														|

***
| Theano | Tensorflow |
|--------|------------|
| 1. More mature since 2008| 1. By Google Brain group, Has Integration with Scikit-learn as skflow.
| 2. Best for Beginner, for Example. Handwriting Recognition: - Dropout, - Backpropagation update, - Softmax output calculation etc helps to understand basic| 2. C++ Based framework, wrappered with Python where each node is Tensor Operation (e.g Matrix add / multiplication, convolutional), A layer can be defined as a composition of these operations.
| 3. Keras, Blocks, Lasagne, Pylearn2 build top of Theano so that it make task more easier for Deep learning and has fency Architecture.| 3. Building Blocks are smaller than caffe - that's why caffe is not defined considered as flexible because for new layer types.
| 4. If anyone wants to code up the entire algorithm for specific problem Theano is the quickest to get started with it gives comprehensive control over Neural Network, best way to prototype them. Ex. SciPy to NumPy , Pylearn2 to Theano.| 4. You have to define full forward, backward, gradient update.
| 5. Theano is very easy as compared to Torch7.| 5. What is worst is that if you want to support both CPU / GPU then you need to support using Implementing extra functions - Forward_GPU, Backwar_GPU.
| 6. Theano uses Symbolic Computation.| 6. Better demonstrate concept like "Cat" can be learned from unlabled youtube images, helped google speech recognition by 25 %, Build Image Search in Google Photos, Automated Image Captioning - DeepDream
| 7. Implemented for most state-of-the-art networks, either in the form of higher level frameworks(Blocks, Keras etc) or in Pure theano.| 7. Has better Computational Graph viz.
| 8. Many attention model / Research Idea started over here.| 8. No - Bidirectional RNN, No - 3D Convolution (Video Recognition)
| | 9. Tensorflow supports C++ interface & library can be compiled / optimized on ARM Architecture because it uses Eign(not BLAs Library) means you can implement model on any devices.
