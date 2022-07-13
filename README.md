# brain-organoid-network-alignment
Using small connected induced subgraphs (graphlets) to align effective connectivity networks derived from cortical organoids.

## Procedure
1. For each time point in a well time series, characterize the nodes based on their directed graphlet-orbit degree vector.\
2a. (Network Aligned Comparison) For each consecutive pair (t, t+1), align nodes based on unnormalized version of node similarity metric. Aligner algorithm was performed with SANA aligner.\
2b. (Non-Network Aligned Comparison) For a given well time series, compare all time points between each other using the directed graphlet-orbit correlation distance.\
2c. (Topological Data Analysis Pt.1) Make a Vietoris-Rips (VR) complex whose metric coincides with the unnormalized node similarity metric, and then compute the persistent homology of the VR complex.\
3. (Topological Data Analysis Pt.2) Compute the persistent path homology of each graph in a well's graph time series. Use the filtration of edge weights going from largest (more important) weights to the smallest (least important) weights.


Testing the git commands.
Hello, foos!