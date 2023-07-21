# Graph-Neural-Networking-Challenge-2023
## Creating-a-Network-Digital-Twin-with-Real-Network-Data

### The goal of this challenge is to create a Network Digital Twin based on neural networks which can accurately estimate QoS performance metrics given the network state and the input traffic. More in detail, solutions must predict the resulting per-flow mean delay given: (i) a network topology (L2 and L3), (ii) a set of input flow packet traces, and (iii) a routing configuration. The following figure presents a schematic representation.

<img src="https://github.com/prathameshk30/Graph-Neural-Networking-Challenge-2023/assets/89546195/2199e6df-1574-4f50-85ce-7843ca1d470e" width=60% height=50%>


### Figure 1: Schematic representation of RouteNet

### As a baseline we provide an open-source implementation of RouteNet: RouteNet-Fermi. This model is the outcome of the three previous editions of the challenge and it has been developed and trained based on simulated data. More importantly for this challenge, it does not support arbitrary packet traces as input.

### RouteNet-Fermi assumes that the input traffic is generated from a stationary stochastic process and uses the moments of such distributions (e.g. mean, variance, etc) as features describing the traffic. In addition, the simulation environment represents an ideal network scenario and RouteNet-Fermi has not been tested with real networks.

### The objective of this challenge is to build a neural network that provides accurate estimates of the mean per-flow delay with a dataset generated from a real network. As a novelty, the dataset contains the input per-flow packet traces. We encourage participants to focus on how to summarize the per-flow packet traces and the non-ideal behavior of real networks. The proposed solution can be based on RouteNet-Fermi, but we also encourage participants to develop their own from-scratch ideas.
