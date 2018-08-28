# Examples

All examples are complete runnable scripts and are self-contained to ease understanding 
(the only exception is dataset fetching that has been moved to [`common.py`](common.py)).

#### 1. Getting Started
 - [**Hello World**](1_1_hello_word_with_mnist.py):
 a very simple example to run your existing model in HyperEngine environment.
 - [**Getting started with tuning**](1_2_getting_started_with_tuning.py):
 tuning a single parameter (`learning_rate`) to find the best value for
 a simple CNN.
 - [**Saving best models**](1_3_saving_best_models_mnist.py):
 tuning several hyper-parameters and saving the best CNN models on the disk.
 - [**Fine-tuning the saved model**](1_4_fine_tuning_saved_model.py):
 training the selected model further to squeeze the highest possible accuracy out of it.
 - [**Learning curve prediction**](1_5_learning_curve_prediction.py):
 optimizing the process with the learning curve prediction.
 - [**Regression problem**](1_6_optimizing_regression.py): HyperEngine is designed for classification problems,
 but with some tricks can be applied in regression settings as well.

#### 2. Convolutional Neural Networks
 - [**Exploring CNN architectures to beat MNIST record**](2_1_cnn_mnist.py):
 exploring and tuning all possible variations of the CNN design to get
 to the [top accuracy](http://rodrigob.github.io/are_we_there_yet/build/classification_datasets_results.html#4d4e495354) 
 for the MNIST dataset.
 - [**Exploring CNN architectures for CIFAR-10 dataset**](2_2_cnn_cifar.py):
 exploring different variations of the CNN design to get good accuracy for the CIFAR-10 dataset
 (state-of-the art accuracy would require a bit more efforts - in the next examples).
 - [**Exploring architectures of All Convolutional Nets for CIFAR-10 dataset**](2_3_all_conv_net_cifar.py):
 exploring different variations of the fully convolutional nets (FCNN), which achieve state-of-the-art accuracy
 with few parameters and computational costs.
 See ["Striving for Simplicity: The All Convolutional Net"](https://arxiv.org/abs/1412.6806) paper for details.

#### 3. Recurrent Neural Networks
 - [**LSTM to classify MNIST digits**](3_1_lstm_mnist.py):
 recurrent neural networks can process images too. Let's see if it can get to 99% with right hyper-parameters.
 - [**RNN to detect SMS spam**](3_2_rnn_sms_spam_detector.py):
 solving a simple NLP problem with different types of RNN. 
 This example shows how hyper-parameters can be used in data processing.

#### 4. Natutal Language Processing
 - [**Word2Vec training**](4_1_word2vec_embedding.py):
 an example of custom data provider to train Word2Vec embedding vectors. In addition, it shows how to use the solver
 without accuracy metric and validation.
 