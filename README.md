# LangChain RAG Project

This project demonstrates how to build a **Retrieval-Augmented Generation (RAG)** system using **LangChain** and **OpenAI GPT**. The RAG system combines the power of **language models** with **document retrieval** to create a more accurate and context-aware response generation process. It allows you to query a database of documents, retrieve relevant information, and generate responses based on that information.

### Key Features:
- **Document Embedding**: Converts documents into embeddings using OpenAI's GPT models.
- **Vector Search**: Uses **Chroma** to store and search document embeddings efficiently.
- **Generative Model**: Utilizes OpenAI GPT to generate text based on the retrieved documents.

## Installation (Windows)

### 1. Install System Dependencies

- **Microsoft C++ Build Tools**: Install from [here](https://github.com/bycloudai/InstallVSBuildToolsWindows?tab=readme-ov-file).
- **onnxruntime**: Install the `onnxruntime` dependency (required by `chromadb`):

  ```bash
  pip install onnxruntime


2. Install Python Dependencies

```python
pip install -r requirements.txt
```

3. Install markdown depenendies with: 

```python
pip install "unstructured[md]"
```

4. Create database

Create the Chroma DB.

```python
python create_database.py
```

5. Query the database

Query the Chroma DB.

```python
python query_data.py "How does Alice meet the Mad Hatter?"
```

Make sure to set your OpenAI API key as an environment variable:

```bash
set OPENAI_API_KEY="your-openai-api-key"
```
