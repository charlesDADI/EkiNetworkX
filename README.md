##EkiNetworkX  - Custom functions to compute networkX graph
========================================================

### This module provides complement functions for lib NetworkX
_Function to  compute bipartite graph and project to one set of nodes_
### __FromDataFrame__ :
* _INPUT:_

    * data is a pandas dataframe
    * u is the name of column  for node 'projected'
    * v is the name of column for node to project
    * w is the name of column for weight
    * alpha is a threshold to map or not a edge    
_OUTPUT:_

	*compute numpy array  (dim 2 N) 
	*U: are nodes projected
	*V: are node to project
	*E: edges with weight attributes if weight columns filled 

- Function to compute graph from a pandas adjancy matrix
NetworkX graphs and project it on one dimension.


Install with pip:

    pip install EkiNetworkX

Example of usage:

    >>> from EkiNetworkX import test1
    >>> proclamer()

Ce code est sous licence WTFPL.