# COVID19NetworkSimulations
Repository for stochastic network simulations of COVID19 dynamics

## Description
Python code used to generate the simulations in, "Dynamics of COVID-19 under social distancing measures are driven by transmission network structure" - Anjalika Nande, Ben Adlam, Justin Sheen, Michael Z. Levy, Alison L. Hill.

We direct users to the iPython notebook, UniformRandomNetwork.ipynb as a starting point. This is a tutorial of sorts where we show how to use the code, describe the different waiting time distributions and give examples of the different plotting functions and interventions that can be simulated. All of the iPython notebooks in this repository were run on Google Colab using GPUs.

## Contents
* networks.py : This file contains functions for the network creation code for both the two and five layer networks.
* seir.py : Contains functions to simulate the stochastic SEIR COVID-19 dynamics on a weighted, directed graph. The code is implemented in JAX, a framework for generating high-performance code optimized to run on GPUs. This file also contains different plotting functions and functions that calculate times to peak infection levels.
* Two_layer_network_sim.ipynb : This iPython notebook was used to analyse the effects of household transmission using the two layer network. Figures 3,4 and 6A in the main text were generated from this file.
* Five_layer_network_sim.ipynb : This iPython notebook was used to analyse the effects of clustered adoption of social distancing measures using the five layer network. Figures 5 and 6B in the main text were generated using this file.
* Relaxing_intervention.ipynb : We used this iPython notebook to analyse the effects of relaxing intervention by merging households. This uses the two layer network and was used to generate Figure 7 in the main text.
