# Travel Planner AI Agent

This repository contains the code for an AI-powered travel planning agent built using the Google Cloud Vertex AI Agent Development Kit (ADK) and the Gemini language model.

## Overview

The Travel Planner AI Agent is designed to help users plan their trips by:

* Gathering their travel preferences (origin, destination, dates, budget).
* Suggesting flight options based on their criteria.
* Suggesting hotel options within their budget and travel dates.
* Providing a summary of the trip details.
* Offering a basic suggested day plan for the destination.

# Steps: 
The below are the following instructions needed to set-up this :
- Frist and the foremost thing to be done is clone or fork (in the top right of this repository `fork`) this repository 
- **Setting up the envoirnment** (Use your terminal):
  ```
  python -m venv .venv  # For Windows or when 'python' points to the correct version
  python3 -m venv .venv # For macOS/Linux
  ```
- **Activating this envoirnment** (Use your terminal):
  
  ```
  # macOS / Linux
  source .venv/bin/activate

  # Windows (CMD)
  .venv\Scripts\activate.bat

  # Windows (PowerShell)
  .venv\Scripts\Activate.ps1
  ```
- The Google-adk package is already installed as you have already cloned this repository ,if not use ```pip install google-adk```
- Create a `.env` file to the parent directory (where this readme.me file is : `/travel_planner/.env`)
- Add the following code to the `.env` file
  ```
  GOOGLE_GENAI_USE_VERTEXAI=FALSE
  GOOGLE_API_KEY=YOUR_API_KEY
  ```
  Note : Replace YOUR_API_KEY with your API-KEY that you have generated from [Google AI Studio](https://aistudio.google.com/), if not click on ```Get API key``` in the top right of the screen and click on `Genrate API Key in new project`.
- You are done with the basic steps, start deploying it in your web by using (Use your terminal) :
  ```
  adk web
  ```
- Open the ```localhost:YOUR_IP_GENERATED``` which the terminal gives you.
## Technologies Used

* **Google Cloud Vertex AI Agent Development Kit (ADK):** Framework for building conversational AI agents.
* **Gemini Language Model:** The underlying AI model powering the agent's natural language understanding and generation.
* **Python:** The primary programming language used.
* **Pydantic:** For data validation and structuring (schemas).

