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

