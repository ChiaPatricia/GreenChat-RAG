# GreenChat-RAG

### Expert-Level Environmental Decision Support

GreenChat is a Retrieval-Augmented Generation (RAG) system specifically designed to provide informed, context-rich assistance for complex environmental decision-making. By integrating dense vector retrieval with a graph-based re-ranking mechanism, it delivers responses that are both scientifically accurate and contextually relevant to environmental queries.

## Overview

GreenChat was developed as my final project of the DS5983 Large Language Models course at Northeastern University. It is designed to help users make informed environmental decisions by providing accurate, context-rich answers. To achieve this, GreenChat uses a two-step process:

1. **Initial Retrieval:** It searches a large dataset of environmental information using dense vector embeddings.
2. **Refinement with a Knowledge Graph:** It then applies a knowledge graph to rank and refine the results based on how concepts relate to each other.

For generating answers, GreenChat relies on a quantized Mistral-7B model. Quantization keeps the system efficient without reducing the quality of responses, making it practical to run on limited computing resources.

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
