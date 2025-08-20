# Conversational AI Chatbot 🤖🛍️

This project demonstrates how to build a conversational AI chatbot using Python, the OpenAI API, and Gradio. The chatbot is designed to act as a helpful assistant in a clothes store, encouraging customers to purchase items that are on sale.

## Features ✨

- **Custom Persona**: The chatbot has a specific "system message" that defines its role and behavior (a clothes store assistant).
- **Sales Promotion**: It is programmed to gently promote hats (60% off) and other items (50% off) to customers.
- **Interactive Interface**: A user-friendly chat interface is created using the Gradio library, allowing for real-time conversation.
- **Local LLM Integration**: The project uses Ollama to run a local language model (`llama3.2`) via the OpenAI API, which is great for development and privacy.

## Prerequisites 🛠️

- Python 3.8+
- [Ollama](https://ollama.ai/) installed and running locally.
- A terminal or command prompt.

## Setup Instructions 🚀

1.  **Clone the repository**:
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    cd your-repo-name
    ```

2.  **Install the required libraries**:
    It's recommended to use a virtual environment.
    ```bash
    pip install -r requirements.txt
    ```

3.  **Set up the environment variables**:
    - Copy the example environment file:
      ```bash
      cp .env.example .env
      ```
    - The code uses Ollama, which typically runs on `localhost` and doesn't require an API key. If you were to use another API, like OpenAI's, you would add your key here. For this project, you can leave the `.env` file as is, but it's good practice to have it for future use.

4.  **Pull the Llama3.2 model with Ollama**:
    Ensure your Ollama server is running, then pull the model from your terminal:
    ```bash
    ollama pull llama3.2
    ```

## How to Run 🏃‍♂️

You can run the chatbot in two ways:

### A. Using the Python Script

Run the `chatbot.py` file directly from your terminal:
```bash
python chatbot.py
