1. Feature engineering is not needed in GNNs, due to the inherent structure of them. The nodes are connnected via links which symbolize the relationships.

### Graph Learning Problems:
#### Node-Level Prediction
 
Node-level problems include:
● Node classification
Predict a property of a node

● Node clustering
Detect if nodes form a community

● Node alignment
Find corresponding nodes in
different graphs

#### Link-Level Prediction

Link-level problems include:

● Link Prediction
Predict whether there are missing links between two
nodes

● Link Regression
Predict continuous values associated with links


#### Graph-Level Prediction

 Subgraph-level problems include:

● Subgraph matching
Predict similarity between graphs
● Subgraph connectivity
Prediction of links between subgraphs


Graph-level problems include:

● Graph classification
● Graph matching
Predict similarity between graphs
● Graph generation


#### Node Embeddings
Why not use a DNN on the adjacency matrix (A) instead?

1. O(|V|) network parameters (bad for large graphs)
2. input graphs would need to have the same size
3. node ordering would be influential

#### Link Prediction Training

![[Pasted image 20240122101805.png]]


