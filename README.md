# The NGLY1 Deficiency Knowledge Graph

This is the repository for the NGLY1 Deficiency Knowledge Graph, the reasoning context to support hypothesis discovery for NGLY1 Deficiency-CDDG (DOID:0060728) research. The user can navigate the knowledge in the graph in the [Neo4j Browser website](http://ngly1graph.org/). This knowledge graph is a structured review around the research question *what is the mechanism underpinning the NGLY1-AQP1 regulation association and explaining the reduced transcriptomic expression of multiple Aquaporins in NGLY1 deficient cells?*. The graph v3.2 is the first deployed in the [Wikibase application](http://ngly1graph.org/contribute/) for community contribution and curation. 


We also provide the related projects on GitHub:
* The [```BioKnowledge reviewer```](https://github.com/NuriaQueralt/bioknowledge-reviewer): a Python library to build structured reviews around NGLY1 Deficiency research questions as knowledge graphs.
* [Neo4j Browser Guides](https://github.com/NuriaQueralt/ngly1-neo4j-guides): the asciidoc/html files and scripts for the creation of our Neo4j Browser Guides to assist the user on the exploration of the graph in Neo4j.
Neo4j.
* [```Krusty```](https://github.com/NuriaQueralt/Krusty): a library to synchronize the NGLY1 Deficiency graph in the **Knowledge Navigation** (Neo4j) and **Knowledge Contribution** (Wikibase) components.
* [Queralt-Rosinach *et al.* 2019](): Manuscript describing the project.

## Data

Versions of the knowledge graph are in the [```neo4j-graphs```](./neo4j-graphs) directory.


## Workflow to create the graph v3.2

To reproduce the creation of the NGLY1 Deficiency knowledge graph v3.2 the user has to run the following workflow. 

##### Prerequisites
* Python 3.
* Jupyter Notebooks framework and the IPython kernel.


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
