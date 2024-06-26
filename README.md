# Computational Neuroscience Tutorial 2024
This tutorial has been designed for the following classes:

- [2023] Brain modelling, AI BSc, UNIMI/PV/B
- [22-23-24] Numerical methods in Neuroscience, Physics MSc, UNIPI, Pisa, Italy
- [21-22-23-24] Biorobotics and Complex Systems, Physics MSc, UNIPI, Pisa, Italy
- [21-22-23] Neural Modeling for Neural Engineering, PhD in Biorobotics, SSSA, Pisa
- [2021] Large Scale Network Simulations, PhD in Neuroscience, INT, Marseille, France

## Introduction to

- Spiking Neural Networks (SNNs) by using PyNN language and/or Brian2 stand-alone simulator

PyNN is a Python library for simulating neural networks. It provides a common interface for a variety of neural simulators, such as NEURON, NEST, and Brian, making it easy to switch between them without having to change the model code. PyNN allows users to define and simulate neural networks using a high-level, neuron-centric interface, similar to the way models are described in neuroscience literature. It is used in many research and education projects to study neural systems, and can be used to simulate models of the brain, as well as artificial neural networks. Brian is a simulator for spiking neural networks. It is written in the Python programming language and is available on almost all platforms. 

- Neural mass modelling with The Virtual Brain simulator 

TheVirtualBrain is a framework for the simulation of the dynamics of large-scale brain networks with biologically realistic connectivity. TheVirtualBrain uses tractographic data (DTI/DSI) to generate connectivity matrices and build cortical and subcortical brain networks. The connectivity matrix defines the connection strengths and time delays via signal transmission between all network nodes. Various neural mass models are available in the repertoire of TheVirtualBrain and define the dynamics of a network node. Together, the neural mass models at the network nodes and the connectivity matrix define the Virtual Brain. TheVirtualBrain simulates and generates the time courses of various forms of neural activity including Local Field Potentials (LFP) and firing rate, as well as brain imaging data such as EEG, MEG and BOLD activations as observed in fMRI. TheVirtualBrain is foremost a scientific simulation platform and provides all means necessary to generate, manipulate and visualize connectivity and network dynamics. In addition, TheVirtualBrain comprises a set of classical time series analysis tools, structural and functional connectivity analysis tools, as well as parameter exploration facilities by launching parallel simulations on a cluster.

## CNT repository on the SpiNNaker neuromorphic system:

1. make the [EBRAINS](https://www.ebrains.eu/news-and-events/addressing-the-mental-health-crisis-with-personalised-treatment-the-launch-of-the-virtual-brain-twin-project?_cldee=z3bx-t-X2WwYH_Ns69VC9kWyaW8VAwaVjMyz-P_vECfCWAdUYljKJvU80RoorvbIqKFnJHI0gre1ubrl7O-BVA&recipientid=contact-48c6764f990ded1182e40022489c5256-e666155866e2475f9b116c5c1ab32fb0&esid=b2e9e86d-e4e2-ee11-904c-002248a43fb1) credentials to access the SpiNNaker server (https://spinn-20.cs.man.ac.uk/hub/login)
1. login on the Jupyter Lab interface
1. install [brian2](https://brian2.readthedocs.io/en/stable/index.html) simulator `pip install brain2`
1. install [PyNN](http://neuralensemble.org/docs/PyNN/installation.html) module `pip install PyNN`
1. install [TVB](https://github.com/the-virtual-brain/tvb-root/tree/master) module `pip install tvb-library tvb-framework`
1. clone this repository `git clone https://github.com/albertoarturovergani/CNT-2024`
1. Open the directory `notebooks/` and run a test with [balance network](notebooks/intro/paper_balance-network.ipynb) by selecting the sPyNNaker kernel
1. if you receive any errors, write to albertoarturo.vergani@santannapisa.it

## Content:

### Overview for the design of Spiking Neural Networks (SNNs)

1. neurons
    - cell types
    - populations
    - recording variables
1. connections
    - synapse types
    - connections types
    - projections
3. simulation managing
    - computational settings
    - save and load outputs
    - visualization tools

### Tutorial notebook

- [CNT notebook](notebooks/intro/CNT_notebook.ipynb)

### Network examples 

- [entry network](notebooks/intro/eg_entry-network.ipynb)
- [single cell](notebooks/intro/eg_single-cell.ipynb)
- [single clique](notebooks/intro/eg_single-clique.ipynb)
- [decaying network](notebooks/intro/eg_decaying-network.ipynb)
- [diverging network](notebooks/intro/eg_diverging-network.ipynb)
- [persistent network](notebooks/intro/eg_persistent-network.ipynb)
- [small-world network](notebooks/intro/eg_small-world-network.ipynb)
- [testing cell models network](notebooks/intro/eg_testing-cell-models-network.ipynb)
- [testing STDP model network](notebooks/intro/eg_testing-STDP-model-network.ipynb)
- [VA_balance network](notebooks/intro/paper_balance-network.ipynb)

### Numerical methods 
- [benchmark on neuron models](notebooks/numerical-methods/)
- [benchmark on network models on Brian2](notebooks/numerical-methods/brian2/)
- [benchmark on network models on TVB](notebooks/numerical-methods/TVB/)

### Knowledge assumptions: 

- basis of spiking neural network theory (https://neuronaldynamics.epfl.ch/online/index.html) or (https://neuromatch.io/academy/)
- familiarity with physical quantities related to electric circuits (e.g., voltages, conductances, currents, etc)
- basic python coding (numpy, work with dictionaries, some matplotlib tools, etc)

### Expected take-home-points: 

- import the simulator
- setup the simulator
- decide the cell types 
- design the populations
- define the synapse types
- select the connection algorithm
- make the projections 
- idealize the stimulus
- run the simulation
- save the results
- recover the results
- postprocessing (visualization, statistics, etc)
- close the simulations

## Links
- [PyNN](http://neuralensemble.org/docs/PyNN/index.html)
- [SpiNNaker](http://apt.cs.manchester.ac.uk/projects/SpiNNaker/)
- [EBRAINS](https://ebrains.eu/)
- [The Human Brain Project](https://www.humanbrainproject.eu/en/)
