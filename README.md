# Computational Neuroscience Tutorial 2024
This tutorial has been designed for the following classes:

- [2023] Brain modelling, AI BSc, UNIMI/PV/B
- [22-23-24] Numerical methods in Neuroscience, Physics MSc, UNIPI, Pisa, Italy
- [21-22-23] Biorobotics and Complex Systems, Physics MSc, UNIPI, Pisa, Italy
- [21-22-23] Neural Modeling for Neural Engineering, PhD in Biorobotics, SSSA, Pisa
- [2021] Large Scale Network Simulations, PhD in Neuroscience, INT, Marseille, France

## Introduction on Spiking Neural Networks (SNNs) by using PyNN language 

PyNN is a Python library for simulating neural networks. It provides a common interface for a variety of neural simulators, such as NEURON, NEST, and Brian, making it easy to switch between them without having to change the model code. PyNN allows users to define and simulate neural networks using a high-level, neuron-centric interface, similar to the way models are described in neuroscience literature. It is used in many research and education projects to study neural systems, and can be used to simulate models of the brain, as well as artificial neural networks.

## PyNN on the SpiNNaker neuromorphic system:

1. make the EBRAINS credentials to access the SpiNNaker server (https://spinn-20.cs.man.ac.uk/hub/login)
1. login on the Jupyter Lab interface
1. install brian2 simulator `pip install brain2`
1. install [PyNN](http://neuralensemble.org/docs/PyNN/installation.html) module `pip install PyNN`
1. clone this repository `git clone https://github.com/albertoarturovergani/CNT-2024`
1. Open the directory `notebooks/` and run a test simulation with [entry-network](notebooks/eg_entry-network.ipynb) by selecting the sPyNNaker kernel

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

- [CNT notebook](notebooks/CNT_notebook.ipynb)

### Network examples 

- [entry network](eg_entry-network.ipynb)
- [single cell](eg_single-cell.ipynb)
- [single clique](eg_single-clique.ipynb)
- [decaying network](eg_decaying-network.ipynb)
- [diverging network](eg_diverging-network.ipynb)
- [persistent network](eg_persistent-network.ipynb)
- [small-world network](eg_small-world-network.ipynb)
- [testing cell models network](eg_testing-cell-models-network.ipynb)
- [testing STDP model network](eg_testing-STDP-model-network.ipynb)
- [VA_balance network](paper_balance-network.ipynb)

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
