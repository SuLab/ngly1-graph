# The NGLY1 Deficiency Knowledge Graph

This is the repository for the NGLY1 Deficiency knowledge graph, the reasoning context to support hypothesis discovery for NGLY1 Deficiency-CDDG research.




## Data

Versions of the knowledge graph are in the ```neo4j-graphs``` directory.


## Workflow to create the graph

To reproduce the creation of the NGLY1 Deficiency v3.2 the user has to run the following workflow:

### Edges

#### Curated network

folder-project: regulation/

run jupyter-notebooks:

    1. `graph_nodes.ipynb`

#### Monarch network

folder-project: monarch/1shell-animal/

run jupyter-notebooks:

    1. `get_monarch_connections.ipynb`

    2. `add_connections_to_net.ipynb`

#### Regulation network

folder-project: regulation/

run jupyter-notebooks:

    1. `regulation.ipynb`

#### RNA expression network

This is a data-driven network built from the NGLY1 knock out transcriptome from fly.

folder-project: regulation/

run jupyter-notebooks:

_Prepare individual expression datasets_:

    1. `./ngly1-fly-chow-2018/chow2018_ngly1_fly_exploratory_analysis.ipynb`

_Build network_:

    2. `transcriptomics.ipynb`

### Graph nodes

folder-project: regulation/

run jupyter-notebooks:

    1. `graph_nodes.ipynb`

### Increase graph connectivity 

folder-project: monarch/1shell-animal/

 run jupyter-notebooks:

    1. `get_monarch_connections_regulation_graph.ipynb`

### Graph edges



## Graph versions

Each graph version is stored.
