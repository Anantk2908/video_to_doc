# video_to_doc


## Introduction

This project is a YouTube Video Summarizer that uses Llama3.1:8B to generate detailed summaries of YouTube videos. Given a YouTube link, the application extracts the audio, transcribes it, and generates a summary document that includes timestamps for easy reference.

The application features a user-friendly Gradio interface where users can input a YouTube link and download the summary document directly

## Installation

1. Ollama
   Make sure is Ollama is installed.
   Then in the terminal use the command ```ollama serve``` to start a ollama server

   After cloning the project make a .env
   Copy the below
   ```env
   OLLAMA_BASE_URL = "http://127.0.0.1:11434/"
   ```

1. Make a python virtual environment
   Use the below command to create a virtual environment
   ```shell
   python3 -m venv <myenvname>
   ```

   Then activate the virtual environment using the command
   ```shell
   source <myenvname>/bin/activate
   ```

2. Install the requirements

   Use the requirements using
   ```shell
   pip install -r requirements.txt
   ```

3. Run the UI

   Use the command
   ```shell
   python app_UI.py
   ```
   This will provide a link which can be opened in the browser


## Scope of Improvement

1. The current implementation works only for the context length of the model that is 128K so implement a vector similarity algorithm to bypass context length limitations
2. Improve the time taken to generate the doc
