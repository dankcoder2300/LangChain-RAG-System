# LangChain RAG Project

This project demonstrates how to build a **Retrieval-Augmented Generation (RAG)** system using **LangChain** and **OpenAI GPT**. The system retrieves relevant documents and generates context-aware responses based on those documents.

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
