# MLOps for EdgeAI

##  1. <a name='Overview'></a>Overview

In this folder, I am revising several MLOps concepts, tools and techniques. The materials are based on the excellent course [Essential Edge AI with Renesas RZ/V2L](https://www.doulos.com/training/ai-and-deep-learning/deep-learning/essential-edge-ai-with-renesas-rzv2l-online/) by Doulos, which I attended in December 2023. Since then, I have used many of the techniques and tools in my own projects at Synthara AG. In the following notebooks, I summarize the key concepts and techniques I learned during the course, as I believe they will come in handy as a reference in the future.

<!-- vscode-markdown-toc -->
* 1. [Overview](#Overview)
* 2. [Getting Started](#GettingStarted)
* 3. [Part 1: Audio Data Preprocessing with SoX](#Part1:AudioDataPreprocessingwithSoX)
* 4. [Part 2: From TensorFlow V2 to TFLite, ONNX and Quantized Models for EdgeAI](#Part2:FromTensorFlowV2toTFLiteONNXandQuantizedModelsforEdgeAI)
* 5. [Part 3: TFLite and ONNX Models for EdgeAI](#Part3:TFLiteandONNXModelsforEdgeAI)
* 6. [Part 4: Object Detection with MobileNet Single Shot Detector (SSD)](#Part4:ObjectDetectionwithMobileNetSingleShotDetectorSSD)
* 7. [Part 5: Object Detection with Quantized Custom CNNs](#Part5:ObjectDetectionwithQuantizedCustomCNNs)
* 8. [Part 6: Model Inference on MQTT, Python Flask and REST APIs](#Part6:ModelInferenceonMQTTPythonFlaskandRESTAPIs)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->

##  2. <a name='GettingStarted'></a>Getting Started

The materials below are organized as either Jupyter Notebooks or Python scripts. To run them, you will need to set up a Python environment as in the [Repository README.md](../README.md). Any additional dependencies are listed in the respective notebooks.

##  3. <a name='Part1:AudioDataPreprocessingwithSoX'></a>Part 1: Audio Data Preprocessing with SoX

As my PhD thought me, data acquisition and preprocessing is a crucial, if not the most important, step in any machine learning project. The majority of my experience lies in 2D and 3D image data, so working with audio data is a less familiar territory for me.

In this notebook, I use the [SoX (Sound eXchange)](https://github.com/chirlu/sox) command line tool to preprocess audio data. I start with a raw audio input file, which I then filter, trim and convert to a spetrogram representation to present to a model for training or inference.

##  4. <a name='Part2:FromTensorFlowV2toTFLiteONNXandQuantizedModelsforEdgeAI'></a>Part 2: From TensorFlow V2 to TFLite, ONNX and Quantized Models for EdgeAI

My daily driver for machine learning is PyTorch, but TensorFlow/Keras is also a very popular framework. I have worked extensively with TensorFlow V1 in my Master's thesis ([see repo here](https://github.com/AndreiRoibu/DeepReinforcementLearning)), but not so much with TensorFlow V2 since it came out.

In this notebook, I revise the key concepts of building and training neural networks with TensorFlow/Keras. These are useful to know, as most EdgeAI models I have encountered are delivered in either TFLite or ONNX format.

I will implement the following toy models:
- Fully Connected Network
- LeNet-style CNN
- LSTM and GRU RNNs

I will also look at how we can implement transfer learning with TensorFlow. This is something I did extensively in PyTorch during my PhD's deep data-fusion experiments, but rarely in TensorFlow.

Platforms like TensorFlow, PyTorch or Keras are great for building and training models, but they are not optimized for deployment on edge devices. For that, we need to convert our models to a more efficient format, such as TFLite or ONNX.

Once we do this, we can use tools like Netron to visualize and inspect the model architecture, layers, parameters and operations, and ONNX Runtime to run inference on the model and check it works well.

Finally, we can also quantize our models to reduce their size and improve their performance on edge devices. This is especially important for TinyML applications, where resources are limited.

##  5. <a name='Part3:TFLiteandONNXModelsforEdgeAI'></a>Part 3: TFLite and ONNX Models for EdgeAI


##  6. <a name='Part4:ObjectDetectionwithMobileNetSingleShotDetectorSSD'></a>Part 4: Object Detection with MobileNet Single Shot Detector (SSD)
##  7. <a name='Part5:ObjectDetectionwithQuantizedCustomCNNs'></a>Part 5: Object Detection with Quantized Custom CNNs
##  8. <a name='Part6:ModelInferenceonMQTTPythonFlaskandRESTAPIs'></a>Part 6: Model Inference on MQTT, Python Flask and REST APIs