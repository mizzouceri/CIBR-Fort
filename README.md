# Smart Grid Knowledge Graph (SG-KG) Research Project

## Overview

This repository contains a comprehensive research project focused on developing a Smart Grid Knowledge Graph (SG-KG) that integrates cybersecurity threat intelligence with power grid infrastructure data. The project combines attack detection methodologies with knowledge graph-based link prediction to enhance smart grid security.

## Project Structure

The repository is organized into two main components:

### 1. Attack Detection (`Attack-detection/`)
This component focuses on developing machine learning models for detecting cyber attacks on smart grid systems.

**Contents:**
- `Dataset1.ipynb`: Initial dataset analysis and preprocessing
- `Dataset2.ipynb`: Extended dataset analysis with additional features
- `Dataset2deployment.ipynb`: Deployment-ready model implementation
- `smart_grid_stability_augmented.csv`: Augmented dataset for training models

### 2. Knowledge Graph Link Prediction (`KG_Link_Pred/`)
This component builds a comprehensive knowledge graph that integrates power grid ontologies with cybersecurity threat intelligence.

**Key Directories:**
- `Ontology/`: Power grid equipment and system ontologies organized by:
  - `Core/`: Fundamental power system components
  - `Generation/`: Generation resources and plants
  - `Prosumers/`: Consumer and prosumer equipment
  - `Wire/`: Transmission and distribution network components

- `Security_KG/`: Cybersecurity knowledge graph data including:
  - MITRE ATT&CK framework entities
  - Attack groups, campaigns, techniques, and mitigations
  - Software and malware information

- `Power_Grid_Ontologies/`: OWL/RDF ontologies for power system modeling
- `Attack_Dataset/`: Power grid connection information and attack scenarios
- `attack-stix-data/`: STIX-formatted threat intelligence data

## Research Objectives

1. **Cyber-Physical Security Integration**: Develop methods to integrate cybersecurity threat intelligence with power grid infrastructure data
2. **Attack Detection**: Create ML models for detecting cyber attacks on smart grid systems
3. **Knowledge Graph Construction**: Build a comprehensive KG linking power grid components with security threats
4. **Link Prediction**: Predict potential attack vectors and vulnerabilities in smart grid systems
5. **Semantic Analysis**: Enable semantic reasoning over cyber-physical relationships

## Key Features

### Knowledge Graph Components
- **Power Grid Ontology**: Comprehensive modeling of power system components using CIM standards
- **Security Ontology**: Integration of MITRE ATT&CK framework with power grid entities
- **Embedding Generation**: Node embeddings for semantic similarity analysis
- **Link Prediction**: Predicting relationships between cyber threats and grid components

### Machine Learning Components
- **Attack Detection Models**: Supervised learning models for anomaly detection
- **Feature Engineering**: Domain-specific features for smart grid security
- **Model Deployment**: Production-ready implementations

## Datasets

### Power Grid Data
- Equipment specifications and configurations
- Network topology and connectivity information
- Operational parameters and measurements

### Cybersecurity Data
- MITRE ATT&CK framework (Enterprise, ICS, Mobile)
- STIX-formatted threat intelligence
- Attack patterns and techniques
- Mitigation strategies

## Methodology

1. **Data Integration**: Combine power grid ontologies with cybersecurity knowledge
2. **Graph Construction**: Build knowledge graphs linking physical and cyber domains
3. **Embedding Learning**: Generate vector representations for semantic analysis
4. **Link Prediction**: Identify potential attack paths and vulnerabilities
5. **Validation**: Evaluate predictions against known attack scenarios

## Usage

### Prerequisites
- Python 3.7+
- Required packages: See individual component requirements

### Getting Started

1. **Attack Detection**:
   ```bash
   cd Attack-detection/
   jupyter notebook Dataset1.ipynb
   ```

2. **Knowledge Graph Construction**:
   ```bash
   cd KG_Link_Pred/
   jupyter notebook Security_KG_Loading.ipynb
   ```

3. **Link Prediction**:
   ```bash
   jupyter notebook Possible\ Link\ Prediction.ipynb
   ```

## Key Notebooks

- `Create_Node_Embeddings.ipynb`: Generate embeddings for KG nodes
- `Similarity_Analysis.ipynb`: Semantic similarity analysis
- `PowerGrid_Ontology_loading.ipynb`: Load and process power grid ontologies
- `load stix security data.ipynb`: Process STIX threat intelligence

## Research Outputs

- **Knowledge Graph**: Integrated cyber-physical knowledge graph
- **Attack Detection Models**: ML models for smart grid security
- **Link Prediction System**: Predictive analytics for threat assessment
- **Semantic Analysis Tools**: Reasoning capabilities over the KG


## License

This project is licensed under the terms specified in the LICENSE file.

## Citation

If you use this work in your research, please cite:
```
@INPROCEEDINGS{11073642,
  author={Neupane, Roshan Lal and Pusapati, Vamsi and Edara, Lakshmi Srinivas and Cheng, Xiyao and Neupane, Kiran and Chintapatla, Harshavardhan and Mitra, Reshmi and Korkali, Mert and Suk Na, Hyeong and Srinivas, Sharan and Calyam, Prasad},
  booktitle={NOMS 2025-2025 IEEE Network Operations and Management Symposium}, 
  title={Securing Inverter-Based Resources via Knowledge-Driven Threat Modeling, Analysis, and Mitigation}, 
  year={2025},
  volume={},
  number={},
  pages={1-9},
  keywords={Threat modeling;Prevention and mitigation;Large language models;Stability criteria;Retrieval augmented generation;Knowledge graphs;Power system stability;Real-time systems;Computer security;Standards;knowledge graph;cybersecurity;inverter-based resources;large language models;retrieval augmented generation},
  doi={10.1109/NOMS57970.2025.11073642}}

```

## Acknowledgments

- MITRE ATT&CK framework for cybersecurity threat intelligence
- CIM standards for power grid modeling
- Research collaborators and funding agencies
