# Alzheimer PPI Network (Systems Biology)

Exploratory analysis of a protein–protein interaction (PPI) network related to Alzheimer’s disease using systems biology and computational approaches. The project uses publicly available interaction data from the STRING database.

## Objective
To identify system-level properties and central proteins (network hubs) within an Alzheimer-related molecular interaction network, as an initial step toward understanding disease-relevant biological mechanisms.

## Background (Why PPI networks?)
Neurodegenerative diseases involve complex molecular processes driven by interactions among many proteins. Modeling these interactions as a network allows us to:
- characterize global network structure,
- identify highly connected proteins (hubs),
- explore potential functional modules (communities),
- generate hypotheses for downstream biological interpretation.

## Data Source
- **STRING database** (Homo sapiens, species ID: 9606)
- Interactions were retrieved via the STRING API using a seed list of Alzheimer-associated genes/proteins.

> Note: This repository does not store large raw datasets. The notebook downloads the network directly from STRING to ensure reproducibility.

## Methods (High-level)
1. Define Alzheimer-related seed genes/proteins.
2. Download the PPI network from STRING with a confidence threshold.
3. Build a graph representation of the network using NetworkX.
4. Compute basic network statistics and identify top hubs by degree.
5. Visualize the network for exploratory inspection.

## Repository Structure
- `01_ppi_network_analysis.ipynb` — main analysis notebook
- `data/` — (optional) local data directory (not tracked if large)
- `figures/` — exported plots and visualizations

## How to Run (Google Colab)
1. Open the notebook in Google Colab.
2. Run the cells in order.
3. The notebook will install required packages, download data from STRING, and generate figures.

## Next Steps
Planned extensions to strengthen the systems biology analysis:
- Community detection to identify functional modules.
- Additional centrality measures (betweenness, eigenvector).
- Sensitivity analysis using different STRING confidence thresholds.
- Mapping hubs/modules to biological processes (pathway enrichment).

## Skills Demonstrated
- Reproducible data acquisition via public APIs
- Data wrangling with Pandas
- Network modeling and analysis with NetworkX
- Scientific reporting and documentation

## Disclaimer
This is an educational and exploratory project. Network centrality does not imply causality.
