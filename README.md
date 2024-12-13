# GreenChat-RAG

### Expert-Level Environmental Decision Support

GreenChat is a Retrieval-Augmented Generation (RAG) system built to deliver detailed, policy-relevant, and scientifically sound answers to complex environmental inquiries. By pairing dense vector retrieval with a graph-based re-ranking layer, GreenChat goes beyond surface-level results to provide responses grounded in the intricate relationships across environmental domains.

## Overview

GreenChat is developed as a final project in the DS5983 Large Language Models course at Northeastern University. It aims to help users navigate the complexities of environmental decision-making. The system works in two stages:

1. **Initial Retrieval:** Quickly identifies a set of relevant documents using dense vector embeddings.
2. **Graph-Based Refinement:** Re-ranks these results through a semantic knowledge graph that highlights key domain relationships.

GreenChat then synthesizes final answers with a quantized Mistral-Instruct 7B model, ensuring efficient inference without sacrificing accuracy or depth. This approach keeps computational requirements manageable, enabling real-world usability even on limited hardware.


## Dataset

The foundation of GreenChat is the GREEN dataset, curated from five distinct environmental categories:

- **Global Climate and Weather**  
- **Renewable Energy**  
- **Environmental Protection**  
- **Environmental Economics**  
- **Natural Technologies**

Each major category (except for Natural Technologies) includes 1,000 balanced samples, providing a broad, representative base of environmental knowledge.

## Requirements

- An NVIDIA L4 GPU or equivalent environment (e.g., Google Colab)
- Python 3.x

**Key Dependencies:**

sentence-transformers
faiss-cpu
networkx>=2.8.4
transformers
torch

## Future Directions

We are actively exploring the following enhancements:

- **Dynamic Knowledge Graph Updates:** Continually integrate new research, policies, and environmental data.
- **Advanced Concept Extraction:** Employ domain-adapted NER models and improved keyword matching.
- **Multilingual Capabilities:** Expand support to multiple languages for broader, more inclusive decision support.
- **Multimodal Data Integration:** Incorporate geospatial, time-series, and visual data sources.
- **Distributed Indexing:** Improve scalability and responsiveness in large-scale deployments.

## Contributing

We welcome contributions! If you wish to propose a major change, please open an issue first so we can discuss it. For smaller fixes or improvements, feel free to submit a pull request directly.

## Acknowledgments

- **Northeastern University, Roux Institute:** For providing the academic environment that nurtured this project.
- **DS5983 Large Language Models Instructors and Peers:** For their valuable guidance and feedback.
- **Open-Source AI Community:** For the tools, resources, and collaborations that made this work possible.

---

*Note: This project was developed for academic and educational purposes.*
