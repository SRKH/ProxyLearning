# Proxy Learning 
The implementation of Proxy Learning presented in "S. R. Kheradpisheh, M. Mirsadeghi, T. Masquelier, Spiking neural networks trained via proxy.", availbale at: https://arxiv.org/abs/2109.13208.

The spiking neural network  is implemented using Spikingjelly package available at https://spikingjelly.readthedocs.io/. The codes are implementded with Spikingjelly version 0.0.0.0.8.

The notebook is adjusted to be run on Google colab. If you are going to run it on your local machine then you can skip the first cell.

## Pretrained model

The pretrained spiking neural (SNN) and its equivalent artificial neural network (ANN) are available in SNN_Params.pt and ANN_Params.pt files, respectively. You can download the pretrained model at https://www.dropbox.com/s/xhg0e2ndesqu5tj/Pretrained.zip?dl=0.

## Paper abstract:

We propose a new learning algorithm to train spiking neural networks (SNN) using conventional artificial neural networks (ANN) as proxy. We couple two SNN and ANN networks, respectively, made of integrate-and-fire (IF) and ReLU neurons with the same network architectures and shared synaptic weights. The forward passes of the two networks are totally independent. By assuming IF neuron with rate-coding as an approximation of ReLU, we backpropagate the error of the SNN in the proxy ANN to update the shared weights, simply by replacing the ANN final output with that of the SNN. We applied the proposed proxy learning to deep convolutional SNNs and evaluated it on two benchmarked datasets of Fahion-MNIST and Cifar10 with 94.56% and 93.11% classification accuracy, respectively. The proposed networks could outperform other deep SNNs trained with tandem learning, surrogate gradient learning, or converted from deep ANNs. Converted SNNs require long simulation times to reach reasonable accuracies while our proxy learning leads to efficient SNNs with much shorter simulation times.
