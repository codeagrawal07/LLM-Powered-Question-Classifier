# ASSESSMENT
- Write a Python script: take a user question, classify it as `factual`, `opinion` , or `math`, and return a response. Share    code on GitHub. Bonus: How would you add API/LLM support?
#  LLM-Powered Question Classifier

This Python project demonstrates how to use a Large Language Model (LLM) to classify a user's question into one of three categories: Math, Opinion, or Factual.

It leverages the LangChain library to interact with Google's Gemini 1.5 Flash model, providing a more intelligent and context-aware classification than simple rule-based systems.

## Description
The script takes a live question from a user and sends it to the Gemini LLM with a specific set of instructions (a "prompt"). The prompt guides the model to analyze the question and determine its category based on predefined rules. This approach allows for flexible and accurate classification without hard-coding complex logic.
## Features
- Intelligent Classification: Utilizes the power of the Gemini 1.5 Flash model to understand the nuances of a user's query.

- LangChain Integration: Uses the popular LangChain framework to structure the prompt, chain the model, and parse the output.

- Interactive Console: Allows for a continuous conversation, prompting the user for questions in a loop.

- Easy to Configure: The model and prompt can be easily modified to change or expand the classification logic.

## Setup and Installation

Before you can run the script, you need to set up your environment and install the required packages.

## Prerequisites
Python 3.7 or higher

A Google API key with the Gemini API enabled.

## 1. Create a Project Folder
Create a new folder for your project and navigate into it.

## 2. Set Up a Virtual Environment (Recommended)

    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate` 
## 3. Create a .env File

You must store your Google API key in an environment file for security. Create a file named `.env` in your project folder and add your key like this:
````GOOGLE_API_KEY="YOUR_API_KEY_HERE"````
## 4. Install Dependencies
Create a file named `requirements.txt` and add the following lines:

```
   langchain-google-genai
   langchain-core
   python-dotenv
```
Now, install these packages using pip:
```
pip install -r requirements.txt
```
## How to Run
Once the setup is complete, you can run the main.py script.

1. Make sure your `main.py`, `.env`, and `requirements.txt` files are in the same project folder.

2. Run the script from your terminal:
```
python main.py
```
3. Interact with the script by typing questions into the console. Type exit to end the session.
## Example Usage
Here is a sample interaction with the script:
```
--- Question Classification Script ---
Ask me a question, or type 'exit' to quit.

You: What is the sum of 500 and 25?
AI Classification: Math

You: Who was the first president of the United States?
AI Classification: Factual

You: What is the best movie of all time?
AI Classification: Opinion

You: exit
Goodbye!
```

    
  






