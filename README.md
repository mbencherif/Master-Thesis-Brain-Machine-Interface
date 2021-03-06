Master's Thesis in the field of neuromorphic information processing for brain-machine interfaces
======================================

## Task: Decoding of 3D Imaginary Reach and Grasp Movements from Non-invasive EEG Signals using Spiking Neural Networks on SpiNNaker Neuromorphic Hardware

--------------------------
## Abstract

Non-invasive, Electroencephalography (EEG) based brain-computer interfaces (BCIs) on motor imagery movements translate the subject’s motor intention into control signals through classifying the EEG patterns caused by di↵erent imagination tasks, e.g. hand movements. This type of BCI has been widely studied and is already used as an alternate mode of communication and environmental control for the disabled, such as patients su↵ering from amyotrophic lateral sclerosis, brainstem stroke and spinal cord injury. Together with recent advancements in neuromorphic computing, which allow real-time, low power implementations of large scale spiking models for data processing, BCI applications could profit from this symbiosis.
Inspired from the architecture of the insect’s olfactory system, we further advance and implement a spiking neural network model (figure below) to decode and predict imaginary movements from EEG signals. The network runs on SpiNNaker, a neuromorphic hardware platform containing 4 chips with 64 cores. To improve the network’s performance a reward based Spike-Time Dependent Plasticity (STDP) learning al- gorithm is implemented and different techniques, as Homeostasis and batch-learning for training the network are tested.
Aiming to find EEG signal components that are stable across imagery movements of the same type we further implemented and analyzed multiple feature extraction techniques as calculating sub-band power, logarithmic band power and motor im- agery specific characteristics from the signal. Additionally we tested the Discrete Wavelet Transform to decompose the EEG data while preserving information from the frequency as well as the time domain. Of all approaches to extract stable char- acteristics the sub-band power features proved to yield the best results. Overall the spiking neural network reaches with the STDP learning algorithm a mean accuracy of 73.4% only falls short by an average of 4.12% in classification rate to state of the art machine learning algorithms. This shows SNNs present a valid alternative to classical machine learning algorithms deployed in BCIs.


--------------------------

## Contents
1. Introduction

2. Basics
* 2.1 EEG based Brain-Computer Interfaces for Motor Imagery
	*	2.1.1 Underlying Brain Processes of Motor Imagery
	*	2.1.2 EEG Data Acquisition of Motor Imagery
* 2.2 NeuromorphicHardwareandAlgorithms
	*	2.2.1 NeuromorphicComputing
	*	2.2.2 NeuromorphicHardware

3. Overview on the State of the Art of EEG based Brain-Machine Interfaces
* 3.1 Review: EEG based Brain-Computer Interfaces
* 3.2 DecodingMethodsofMotorImageryfromEEGData
* 3.3 Spiking Neural Network based on the Insect’s Olfactory System

4. Solution Design
* 4.1 Design
* 4.2 ExperimentalData

5. Implementation
* 5.1 DataPreprocessing
* 5.2 FeatureExtractionMethods
	* 5.2.1 Event Related Desynchronization and Synchronization 
	* 5.2.2 DiscreteWaveletTransform
	* 5.2.3 Feature Processing: Cross-Trial Encoding
	* 5.2.4 Results:FeatureExtraction
*5.3 SpikingNeuralNetworkImplementation
	* 5.3.1 FeatureEncoding
	* 5.3.2 NetworkImplementation
	* 5.3.3 NetworkEvaluation
	* 5.3.4 Results:SpikingNeuralNetwork

6. Discussion

7. Conclusion



--------------------------


Link to the full text thesis:
<br />
[THESIS](https://github.com/LeRyc/Master-Thesis-Brain-Machine-Interface/blob/master/Report_Final/Thesis.pdf)


--------------------------

Architecture of the olfactory based spiking neural network:
<img src="https://github.com/LeRyc/Master-Thesis-Brain-Machine-Interface/blob/master/readme_img/snn_architecture.png" width="400">




