# GreenChat-RAG

### An Environmental Decision Support RAG System

GreenChat is a sophisticated Retrieval-Augmented Generation (RAG) system designed to provide expert-level environmental decision support. By combining advanced dense vector retrieval with graph-based re-ranking, GreenChat delivers contextually grounded, scientifically accurate responses to complex environmental queries.

## About

This project was developed as a final project for DS5983 Large Language Models at Northeastern University. It addresses the growing need for specialized AI systems in environmental decision-making by integrating domain-specific knowledge with state-of-the-art language models.

GreenChat employs a two-stage retrieval framework that leverages both embedding-based semantic representations and a graph-structured knowledge model. At its core, the system uses a 4-bit quantized Mistral-7B model, optimized for efficient, high-quality response generation while maintaining computational efficiency.

## Dataset

The GREEN dataset forms the foundation of our system, carefully curated from five distinct environmental categories:
- Global Climate and Weather
- Renewable Energy
- Environmental Protection
- Environmental Economics
- Natural Technologies

Each category (except Natural Technologies) contains 1,000 balanced samples, ensuring comprehensive coverage across environmental domains.

## Requirements

- NVIDIA L4 GPU or equivalent
- Google Colab environment
- Python 3.x
- Key dependencies:
  ```
  sentence-transformers
  faiss-cpu
  networkx>=2.8.4
  transformers
  torch
  ```

## Future Development

We are actively working on several enhancements:
- Implementation of dynamic knowledge graph updates
- Enhanced concept extraction capabilities
- Extended multilingual support
- Integration of multimodal data
- Development of distributed indexing systems

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## Acknowledgments

- Northeastern University, Roux Institute
- DS5983 Large Language Models course instructors and peers
- The open-source AI community for their invaluable tools and resources

---
*Note: This project is part of academic coursework and is intended for educational purposes.*
