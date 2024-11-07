# NVIDIA-RAG-Document-Search

This project is a **Retrieval-Augmented Generation (RAG) application** developed using **Nvidia NIM** and **LangChain** with a **Streamlit** interface. It enables document embeddings and similarity-based question answering, designed around an 8th-grade textbook as a knowledge base.

## Features

- **NVIDIA Embeddings**: Utilizes Nvidia NIM for document embeddings, enabling semantic search.
- **LangChain Integration**: Creates efficient document retrieval and chaining for response generation.
- **FAISS Vector Store**: Stores document embeddings in a vector database to facilitate similarity search.
- **Streamlit Interface**: User-friendly interface for query input and output display, making it easy to interact with the application.

## Project Structure

- **main.py**: The main Streamlit app file containing the code for document embeddings, vector store setup, and query processing.
- **8th_class_book/**: Directory containing PDF files used as the document source.
- **requirements.txt**: Lists required Python packages for the project.

## Setup

### Prerequisites

- Python 3.8 or higher
- Nvidia API Key (stored in `.env` file)

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/GirishVenkataramana/NVIDIA-RAG-Document-Search.git
   cd NVIDIA-RAG-Document-Search
   ```

2. **Create and activate a virtual environment**:
   ```bash
   python -m venv nim-env
   source nim-env/bin/activate   # On Windows, use `nim-env\Scripts\activate`
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Add your Nvidia API Key**:
   - Create a `.env` file in the root directory and add your key:
     ```
     NVIDIA_API_KEY=your_nvidia_api_key
     ```

### Running the App

To launch the Streamlit app, run:
```bash
streamlit run main.py
```

## Usage

1. **Document Embedding**: Click the "Document Embedding" button to embed the documents and store them in the FAISS vector database.
2. **Ask Questions**: Enter your question based on the 8th-grade content in the input box and click "Submit." The app will retrieve relevant document context and generate an answer.
3. **Document Similarity Search**: Explore relevant document chunks to see where the answer was derived.

## Example

![Example Screenshot](link_to_screenshot)

## Technologies Used

- **NVIDIA NIM**: For embeddings and NLP tasks.
- **LangChain**: Streamlines document chaining and response generation.
- **Streamlit**: Provides a simple, interactive web interface.
- **FAISS**: Vector database for efficient similarity search.

## License

This project is licensed under the MIT License.

