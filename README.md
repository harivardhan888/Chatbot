# Q&A Chatbot Suite (OpenAI, Ollama)

This repository contains Streamlit-based chatbot application built using LangChain. One chatbot uses OpenAI GPT models and can be deployed online, while the other uses local Ollama models and runs offline on your machine.

## Live Demo (OpenAI)
https://chatbot-openai888.streamlit.app

## Project Structure
QA_Chatbot/
├── app_openai.py
├── app_ollama.py
├── requirements.txt
├── .env
├── venv/
└── README.md

## Features
OpenAI Chatbot:
- Uses GPT-4o, GPT-4 Turbo, GPT-4
- Streamlit UI with model, temperature, token controls
- Uses LangChain ChatOpenAI + ChatPromptTemplate + StrOutputParser
- Deployable on Streamlit Cloud

Ollama Chatbot:
- Works offline using local LLMS (Gemma, Mistral, etc.)
- Uses LangChain Ollama integration
- Only works locally or on your own server (not Streamlit Cloud)


## Run the Apps
Run OpenAI chatbot:
streamlit run app_openai.py

Run Ollama chatbot:
Install Ollama from https://ollama.com
ollama pull gemma:2b
streamlit run app_ollama.py

## Dependencies
streamlit  
openai  
langchain  
langchain-openai  
langchain-core  
langchain-community  
python-dotenv  

Install all using:
pip install -r requirements.txt

## API Keys
Only OpenAI chatbot needs an API key. OLLAMA version runs offline. 

## Contributing
Pull requests are welcome.

## Support
If you like this project, give it a star ⭐ on GitHub.
