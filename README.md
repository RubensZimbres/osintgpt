<div align="center">

# **OSINT GPT**
<br />

---

<br />

[![GitHub forks](https://img.shields.io/github/forks/estebanpdl/osintgpt.svg?style=social&label=Fork&maxAge=2592000)](https://GitHub.com/estebanpdl/osintgpt/network/)
[![GitHub stars](https://badgen.net/github/stars/estebanpdl/osintgpt)](https://GitHub.com/estebanpdl/osintgpt/stargazers/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/estebanpdl/osintgpt/blob/main/LICENCE)
[![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://twitter.com/estebanpdl)
[![Made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
[![Twitter estebanpdl](https://badgen.net/badge/icon/twitter?icon=twitter&label)](https://twitter.com/estebanpdl)

---

</div>

<br />

`osint-gpt` is a Python package for leveraging OpenAI's GPT models to analyze text data and perform tasks such as calculating text embeddings, searching for similar documents, and more. It is designed for use in open-source intelligence (OSINT) applications and research.

<hr />
<br />



## **Disclaimer**

The "osint-gpt" tool is provided for research purposes and intended to assist users in analyzing data from open-source intelligence (OSINT) tools more efficiently. It relies on third-party services, such as the OpenAI API, various database engines, and other resources that may have associated costs. By using this tool, you acknowledge that you are responsible for understanding and managing any costs related to these services. The creators and maintainers of "osint-gpt" are not liable for any expenses incurred or any misuse of the tool. Please use this tool responsibly and in compliance with all applicable laws and regulations.

<hr />
<br />

## **Requirements**



<hr />
<br />

## **Installation**

You can install the `osint-gpt` package using pip:

```bash
pip install osint-gpt
```


<br />
<hr />
<br />

## **Quick Start**

<br />


Setup your environment variables: Create a `.env` file with your OpenAI API key and GPT model name:

```
OPENAI_API_KEY=your_openai_api_key
OPENAI_GPT_MODEL=model_name
```

<hr />
<br />

### **`Embeddings`**

<br />

1. Import the package and create an `OpenAIEmbeddingGenerator` instance:

```python
from osintgpt.embedding import OpenAIEmbeddingGenerator

args = {
    'env_file_path': './config/.env'
}

embedding_generator = OpenAIEmbeddingGenerator(**args)
```

2. Load your text data:

```python
data = ["Text 1", "Text 2", "Text 3"]
embedding_generator.load_strings(data)
```

3. Calculate embeddings:

```python
embeddings = embedding_generator.embeddings
```


<hr />
<br />

### **`Vector store`**

<br />

1. **Qdrant**

[Qdrant](https://qdrant.tech/) is a high-performant vector search database written in Rust.

<hr />
<br />


## **Features**

- Easy loading of text data
- Text embeddings calculation
- Embeddings generation for new text


<hr />
<br />



