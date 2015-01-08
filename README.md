##EkiNetworkX  - Custom functions to compute networkX graph


========================================================
### INSTALL
Install with pip:

    pip install ekiNx

Example of usage:

    >>> from ekiNx import core
    >>> core.proclamer()
========================================================

### This module provides complement functions for lib NetworkX
_Function to  compute bipartite graph and project to one set of nodes_
#### __FromDataFrame__ :
* _INPUT:_

    * data is a pandas dataframe
    * u is the name of column  for node 'projected'
    * v is the name of column for node to project
    * w is the name of column for weight
    * alpha is a threshold to map or not a edge    
* _OUTPUT:_

	* compute numpy array  (dim 2 N) 
	* U: are nodes projected
	* V: are node to project
	* E: edges with weight attributes if weight columns filled 

#### __mapBipartite__ :
- create biGraph and map nodes/edges
* _INPUT:_
    * U nodes 'projected'
    * V nodes to project
    * E: edges with weight attributes if weight columns filled 
* _OUTPUT:_
    * g: networkX biGraph 

#### __projectGraph__ :
- create biGraph and map nodes/edges
* _INPUT:_
    * U    biGraph a bigraph networkX object 
    * V is the set on
	* weight_function  to compute edges weight ( for instance jaccard)
* _OUTPUT:_
    * g: networkX object representing a undirected graph



#### __graphFromPandasAdjancyMatrix__ :
- map nodes and edges from adjancy matrix:
* _INPUT:_
    * data is a pandas object representing an adjacency matrix
* _OUTPUT:_
    * g: anetworkX object representing a undirected graph
        each node contain is label with column label

========================================================

Ce code est sous licence WTFPL.