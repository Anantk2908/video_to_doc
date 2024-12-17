# SummarizeTube

## Introduction

This project is a YouTube Video Summarizer that uses **Gemini 1.5 Pro** to generate detailed summaries of YouTube videos. Given a YouTube link, the application extracts the audio, transcribes it, and generates a summary document that includes timestamps for easy reference.

The application features a user-friendly Gradio interface where users can input:
- A YouTube link
- Their **Gemini 1.5 Pro API Key**

The summary document can be downloaded directly from the UI.

---

## Installation

1. **Retrieve Gemini 1.5 Pro API Key**
   - Go to [Google AI Studio](https://aistudio.google.com/).
   - Sign in with your Google account and create a new project.
   - Generate an **API Key** for Gemini 1.5 Pro.
   - Keep this key ready; it will be entered directly into the UI.

2. **Create a Python virtual environment**
   - Use the below command to create a virtual environment:
     ```shell
     python3 -m venv <myenvname>
     ```
   - Activate the virtual environment:
     ```shell
     source <myenvname>/bin/activate
     ```

3. **Install the requirements**
   - Install the required libraries:
     ```shell
     pip install -r requirements.txt
     ```

4. **Run the UI**
   - Start the Gradio UI using the following command:
     ```shell
     python app_UI.py
     ```
   - This will provide a link that can be opened in the browser.

5. **Generate Summary Document**
   >![Alt text](assets/UI.png)
   - As prompted in the give the youtube link that you can want summarize and the API from the previous step
   - After the code has completed running you will get a document.

6. **Sample Output**

   Here is an example summary document generated by the application for the video:

   #### Video Details:
   - **Video Title**: [The Cognitive Tradeoff Hypothesis](https://www.youtube.com/watch?v=ktkjUjcZid0)  
   - **Channel**: Vsauce  

   #### Sample Summary Document:  
   [Download Summary Document](https://github.com/Anantk2908/video_to_doc/raw/main/assets/Chimpanzee_Memory_vs_Human_Language.docx)

---

Feel free to download the document and explore the results!


