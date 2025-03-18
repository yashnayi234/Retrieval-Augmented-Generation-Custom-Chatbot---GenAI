# Retrieval-Augmented-Generation-Custom-Chatbot GenAI

## Financial RAG Chatbot

This repository demonstrates a Retrieval-Augmented Generation (RAG) approach for building a domain-specific chatbot using financial data. The chatbot leverages OpenAI's API and embedding techniques to provide accurate, context-rich responses to financial queries by integrating relevant information from a curated financial dataset.

## Features

- **Contextual Response Generation:**  
  Enriches user queries with relevant financial context extracted from a domain-specific dataset.

- **Efficient Retrieval:**  
  Uses cosine similarity on embeddings to select the most relevant data entries, ensuring precise and informed responses.

- **Customizable Prompt Construction:**  
  Dynamically builds prompts based on the token budget using a flexible prompt template, allowing control over the amount of context provided.

- **Seamless Integration with OpenAI API:**  
  Combines pre-trained models and fine-tuned data to generate high-quality answers for financial queries.

## Getting Started

### Prerequisites

- Python 3.7 or higher
- [OpenAI Python library](https://github.com/openai/openai-python)
- [Pandas](https://pandas.pydata.org/)
- [tiktoken](https://github.com/openai/tiktoken) (for token counting)
- [SciPy](https://www.scipy.org/) (for computing cosine similarity)
- Jupyter Notebook (optional, for interactive development)

### Installation

1. **Clone the Repository:**

   ```bash
   git clone <https://github.com/yashnayi234/Retrieval-Augmented-Generation-Custom-Chatbot---GenAI.git>
   cd <https://github.com/yashnayi234/Retrieval-Augmented-Generation-Custom-Chatbot---GenAI>


```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate


pip install -r requirements.txt


## Usage

### Data Preparation

- Place your financial dataset (e.g., `finanical_rag_embedding_dataset.csv`) into the `data/` folder.
- Ensure the dataset includes a text column (such as `text` or `context`) and, if possible, precomputed embeddings.

### Running the Notebook

- Open `project.ipynb` in your preferred Jupyter environment.
- Follow the notebook steps to:
  - Load and preprocess the dataset.
  - Compute embeddings for the dataset (if not precomputed).
  - Build context-aware prompts using relevance ranking.
  - Generate responses for financial questions using the OpenAI API.

### Interactive Querying

- The notebook provides functions for both basic and RAG-enhanced queries. Experiment by inputting different financial queries to see how the chatbot leverages the dataset for context-aware responses.

## Customization

- **Prompt Template:**  
  Modify the prompt template within the code to adjust how context and questions are combined.
  
- **Token Limits:**  
  Customize `max_prompt_tokens` and `max_answer_tokens` in the notebook to balance between context richness and response length.
  
- **Dataset:**  
  Replace or update the financial dataset with other domain-specific data as needed. Ensure that the data is preprocessed for embedding generation.

## Contributing

- Contributions to improve the Financial RAG Chatbot are welcome! Please fork the repository, make your changes, and submit a pull request with a detailed description of your improvements.

## License

- This project is licensed under the MIT License. See the `LICENSE` file for further details.

## Contact

- For questions or support, please open an issue in the repository or contact [your.email@example.com](mailto:your.email@example.com).


