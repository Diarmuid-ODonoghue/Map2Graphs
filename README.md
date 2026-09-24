# Homomorphic Graph Search - HOGS

## HOGS algorithm for Largest Common Edge Subgraph between 2 graphs
### Unlabeled or - with labels on edges and/or nodes.
### 2 versions available

Two versions of the graph mapping algorithm called HOGS - Homomorphic Graph Search.
Find the largest common edge subgraph, between two graphs.
Uses the Erdos Renyii graph generator.
Also: 3 versions of knowledge graphs derived from human Analogy experiments - **Analogy Materials Corpus**. 

Details forthcoming.

**nx.isomorphVF2cb(G1, G1)** - with *Conor Brady*

An instrumented version of the famous VF2 algorithms. Adapted for subgraph isomorphism and works on MultiDiGraphs in NetworkX. 
Example code:

`G1 = nx.from_edgelist([('a','b'), ('b','c')])`

`G2 = nx.from_edgelist([(1,2)])`

`GM = MultiDiGraphMatcher(G1, G2)`

`print(GM.mapping)`

returns the dictionary: `{'a': 1, 'b': 2}`

**Restrict the allowed node-to-node mappings**
To restrict the space of feasible mapping, change `semantic_feasibility(self, G1_node, G2_node)`
