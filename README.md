# GreenChat-RAG

### Expert-Level Environmental Decision Support

GreenChat is a Retrieval-Augmented Generation (RAG) system specifically designed to provide informed, context-rich assistance for complex environmental decision-making. By integrating dense vector retrieval with a graph-based re-ranking mechanism, it delivers responses that are both scientifically accurate and contextually relevant to environmental queries.

## Overview

Developed as a final project for the DS5983 Large Language Models course at Northeastern University, GreenChat addresses the growing need for specialized AI solutions in environmental science and policy. The system employs a two-stage retrieval strategy—first using embedding-based semantic search, then refining results through a knowledge graph—to ensure that output is both precise and grounded in established environmental domains.

At its core, GreenChat utilizes a 4-bit quantized Mistral-7B model, striking an optimal balance between efficiency and response quality. This approach ensures that resource constraints need not compromise the depth or accuracy of environmental insights.

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
