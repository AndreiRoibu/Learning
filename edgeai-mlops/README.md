# MLOps for EdgeAI

##  1. <a name='Overview'></a>Overview

In this folder, I am revising several MLOps concepts, tools and techniques. The materials are based on the excellent course [Essential Edge AI with Renesas RZ/V2L](https://www.doulos.com/training/ai-and-deep-learning/deep-learning/essential-edge-ai-with-renesas-rzv2l-online/) by Doulos, which I attended in December 2023. Since then, I have used many of the techniques and tools in my own projects at Synthara AG. In the following notebooks, I summarize the key concepts and techniques I learned during the course, as I believe they will come in handy as a reference in the future.

<!-- vscode-markdown-toc -->
* 1. [Overview](#Overview)
* 2. [Getting Started](#GettingStarted)
* 3. [Part 1: Audio Data Preprocessing with SoX](#Part1:AudioDataPreprocessingwithSoX)
* 4. [Part 2: Training Networks with Tensorflow: Fully Connecteded, CNNs, RNNs, LSTMs and GRUs](#Part2:TrainingNetworkswithTensorflow:FullyConnectededCNNsRNNsLSTMsandGRUs)
* 5. [Part 3: Models for EdgeAI with TFLite and ONNX](#Part3:ModelsforEdgeAIwithTFLiteandONNX)
* 6. [Part 4: Model Inferencing with TFLite and ONNX Runtimes](#Part4:ModelInferencingwithTFLiteandONNXRuntimes)
* 7. [Part 5: Quantization for TinyML](#Part5:QuantizationforTinyML)
* 8. [Part 6: Object Detection with MobileNet Single Shot Detector (SSD)](#Part6:ObjectDetectionwithMobileNetSingleShotDetectorSSD)
* 9. [Part 7: Object Detection with Quantized Custom CNNs](#Part7:ObjectDetectionwithQuantizedCustomCNNs)
* 10. [Part 8: Model Inference on MQTT, Python Flask and REST APIs](#Part8:ModelInferenceonMQTTPythonFlaskandRESTAPIs)

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

##  4. <a name='Part2:TrainingNetworkswithTensorflow:FullyConnectededCNNsRNNsLSTMsandGRUs'></a>Part 2: Training Networks with Tensorflow: Fully Connecteded, CNNs, RNNs, LSTMs and GRUs
##  5. <a name='Part3:ModelsforEdgeAIwithTFLiteandONNX'></a>Part 3: Models for EdgeAI with TFLite and ONNX
##  6. <a name='Part4:ModelInferencingwithTFLiteandONNXRuntimes'></a>Part 4: Model Inferencing with TFLite and ONNX Runtimes
##  7. <a name='Part5:QuantizationforTinyML'></a>Part 5: Quantization for TinyML
##  8. <a name='Part6:ObjectDetectionwithMobileNetSingleShotDetectorSSD'></a>Part 6: Object Detection with MobileNet Single Shot Detector (SSD)
##  9. <a name='Part7:ObjectDetectionwithQuantizedCustomCNNs'></a>Part 7: Object Detection with Quantized Custom CNNs
##  10. <a name='Part8:ModelInferenceonMQTTPythonFlaskandRESTAPIs'></a>Part 8: Model Inference on MQTT, Python Flask and REST APIs