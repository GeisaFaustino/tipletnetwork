# A Simple Triplet Neural Network (TNN) Implementation

Here you will find a simple triplet network implementation for signature validation purposes using Keras.

The code is inspired from KinWaiCheuk [github repository](https://github.com/KinWaiCheuk/Triplet-net-keras). For a good intruduction about Triplet net (also know as triplet loss) see [Triplet Loss and Online Triplet Mining in TensorFlow](https://omoindrot.github.io/triplet-loss) by Olivier Moindrot.

As mentioned above, we are using triplet NN to validade signatures. The idea is that:

* Two examples of genuine signatures from the same person have their embeddings close together in the embedding space;
* A genuine signature and a forged one have their embeddings far away.

For comparison purposes we also generate embeddings using a trained network, the VGG16. 

We use this open-source [dataset](https://cedar.buffalo.edu/NIJ/data/signatures.rar) for training and testing our network.

Our approach can be divided into:
 * Download the dataset and extract it to appropriate folder. 
 * Prepare dataset, generate triples and divide dataset in two subsets trainning and validation (or testing).
 * Train network
 * Compare results


**References**:

* [Tensorflow-Signature-Recognition](https://github.com/rmalav15/signature-recognition)
* [Triplet Loss - Coursera video](https://www.coursera.org/lecture/convolutional-neural-networks/triplet-loss-HuUtN?utm_source=linkshare&siteID=je6NUbpObpQ-vGHsrqsSjAzy9re5xFJZ7Q&ranEAID=je6NUbpObpQ&utm_content=10&ranMID=40328&ranSiteID=je6NUbpObpQ-vGHsrqsSjAzy9re5xFJZ7Q&utm_campaign=je6NUbpObpQ&utm_medium=partners)
* [How to Save and Load Your Keras Deep Learning Model](https://machinelearningmastery.com/save-load-keras-deep-learning-models/)
