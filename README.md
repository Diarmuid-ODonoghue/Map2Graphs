### Homomorphic Graph Search - HOGS
### HOGS algorithm for Largest Common Edge Subgraph between 2 graphs
### Unlabeled or - with labels on edges and/or nodes.
2 versions available

Two versions of the graph mapping algorithm called HOGS - Homomorphic Graph Search.
Find the largest common edge subgraph, between two graphs.
Uses the Erdos Renyii graph generator.
Also: 3 versions of knowledge graphs derived from human Analogy experiments - **Analogy Materials Corpus**. 

### Subgraph - Graph isomorphism

`nx.isomorphVF2cb(G1, G1)` - with *Conor Brady*

The `isomorphvf2cb.py` file offers an instrumented version of the famous VF2 algorithms, relying only on the NetworkX package. VF2 has been modified for subgraph isomorphism and works on MultiDiGraphs under NetworkX. 
Example code:

`G1 = nx.from_edgelist([('a','b'), ('b','c')])`

`G2 = nx.from_edgelist([(1,2)])`

`GM = MultiDiGraphMatcher(G1, G2)`

`print(GM.mapping)`

returns the dictionary: `{'a': 1, 'b': 2}`

**Restrict the allowed node-to-node mappings**
To restrict the space of feasible mapping, change `semantic_feasibility(self, G1_node, G2_node)`


**References**

Luigi P. Cordella, Pasquale Foggia, Carlo Sansone, Mario Vento, “A (Sub)Graph Isomorphism Algorithm for Matching Large Graphs”, IEEE Transactions on Pattern Analysis and Machine Intelligence, vol. 26, no. 10, pp. 1367-1372, Oct., 2004. 

L. P. Cordella, P. Foggia, C. Sansone, M. Vento, “An Improved Algorithm for Matching Large Graphs”, 3rd IAPR-TC15 Workshop on Graph-based Representations in Pattern Recognition, Cuen, pp. 149-159, 2001. 
