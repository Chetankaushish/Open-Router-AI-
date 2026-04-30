# OpenRouter AI Agent

This project is a simple AI assistant built using Python, Jupyter Notebook, and OpenRouter API. It demonstrates how to connect multiple free AI models with Python using the OpenAI SDK and generate intelligent responses through prompt-based interaction.

---

# Features

* OpenRouter API integration
* Access to multiple free AI models
* AI chatbot functionality
* Prompt-based response generation
* Beginner-friendly implementation
* Works with Jupyter Notebook and VS Code

---

# Technologies Used

* Python
* OpenRouter API
* OpenAI Python SDK
* Jupyter Notebook
* VS Code

---

# Supported Models

This project can work with different free AI models available on OpenRouter, such as:

```python
meta-llama/llama-3.1-8b-instruct:free
google/gemma-2-9b-it:free
mistralai/mistral-7b-instruct:free
```

---

# Installation

Install the required library:

```bash
pip install openai
```

---

# Setup API Key

Create your free OpenRouter API key:

[https://openrouter.ai/keys](https://openrouter.ai/keys)

Replace:

```python
api_key="YOUR_OPENROUTER_API_KEY"
```

with your own API key.

---

# Example Code

```python
from openai import OpenAI

client = OpenAI(
    base_url="https://openrouter.ai/api/v1",
    api_key="YOUR_OPENROUTER_API_KEY"
)

response = client.chat.completions.create(
    model="meta-llama/llama-3.1-8b-instruct:free",
    messages=[
        {
            "role": "user",
            "content": "What is Artificial Intelligence?"
        }
    ]
)

print(response.choices[0].message.content)
```

---

# Future Improvements

* Voice assistant integration
* Streamlit web chatbot
* AI memory support
* Multi-model comparison
* File and PDF analysis
* AI coding assistant

---

# Important Security Note

Do not upload your real API key to GitHub.

Use:

```python
YOUR_OPENROUTER_API_KEY
```

instead of your real key.

---

# Author

Chetan Sharma

---

# License

This project is created for learning and educational purposes.
