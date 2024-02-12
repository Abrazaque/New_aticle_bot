### Instant Article Research Tool

This repository contains the source code for the Instant Article Research Tool, a Streamlit web application designed to streamline the process of researching articles. Using OpenAI's powerful models and the LangChain library, this tool allows users to input URLs for articles and ask questions, receiving summarized answers based on the content of those articles.

## Features

- **URL Input**: Users can input up to three URLs in the sidebar, pointing to the articles they wish to research.
- **Question Processing**: After processing the URLs, users can input a question related to the articles' content, receiving a concise answer.
- **Source Citing**: Along with the answer, the tool provides sources from the articles, enhancing credibility and traceability.

## How It Works

The application uses the following process:
1. **Data Loading**: Loads the content from the specified URLs.
2. **Text Splitting**: Splits the loaded text into manageable chunks for processing.
3. **Embedding & Vector Store Creation**: Generates embeddings for the text and creates a vector store using FAISS for efficient retrieval.
4. **Question Answering**: Processes the user's question through a retrieval and question-answering chain, leveraging OpenAI's models.

## Prerequisites

- Python 3.6+
- Streamlit
- LangChain
- OpenAI API Key

## Installation

1. Clone this repository.
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Streamlit application:
   ```bash
   streamlit run main.py
   ```

## Usage

After launching the app, follow the instructions in the sidebar to input URLs and ask questions based on the articles' content.

## Contributing

We welcome contributions to improve the Instant Article Research Tool. Feel free to fork the repository, make your changes, and submit a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- OpenAI for the GPT models.
- The LangChain library for facilitating the development of language applications.

---
