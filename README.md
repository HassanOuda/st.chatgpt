# st.chatgpt
Streamlit app for chatGPT for connecting to your own LLM and your own function/agent

## Screenshot

![alt text](assets\app.png "App")

## LLMs

Currently the app only supports Vertex AI PaLM models

You need 2 parameters to use PaLM:
- a GCP project
- a service account key from that project that has access to the PaLM api


## How to get started

Install following python packages:
```
pip install -r requirements.txt
```

Run these commands to start the app:
```
cd app
export PROJECT_ID="gcp_project_id"
export CREDENTIALS=key.json
py -m streamlit run ./main.py
```
## Roadmap

- Add OpenAI LLM 
- Other LLMs support
- Add LLM Cache
- Add LLM serialization