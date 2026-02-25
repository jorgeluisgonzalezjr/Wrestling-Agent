# 🎙️ WWE AI Assistant: The Michael Cole GUI Agent

A custom-built, interactive Graphical User Interface (GUI) AI agent designed specifically for professional wrestling fans. 

Powered by the persona of legendary WWE commentator Michael Cole, this desktop assistant goes beyond basic chatbots. Not only does it answer deep-cut wrestling trivia and historical inquiries, but it acts as a personal event concierge—helping fans track down the next live shows, plan their trips, and get real-time weather forecasts for the venues.

## ✨ Key Features
* **Interactive GUI:** A clean, user-friendly graphical interface that makes chatting with the agent feel like a seamless desktop app.
* **Ultimate Wrestling Trivia:** Programmed with extensive system instructions to mimic Michael Cole's commentary style, complete with dynamic tone shifts depending on whether he's discussing a Heel or a Face.
* **Live Event Tracking:** Uses real-time web search to find upcoming Raw, SmackDown, and Premium Live Event schedules.
* **Trip Planning & Weather:** Integrates geocoding and live weather APIs so fans know exactly what the forecast looks like in the city where the event is hosted.

## 🛠️ Built With
This project leverages custom tool-calling to connect the AI's reasoning to real-world data:
* **OpenAI API (gpt-4o):** Powers the core conversational engine and dynamic persona.
* **SerpAPI:** Enables live web scraping to fetch real-time event schedules and breaking wrestling news.
* **Python Agents Framework:** Handles the asynchronous execution of specific tools (`web_search`, `geocode`, `get_weather`).

## 📸 Interface 


<img width="796" height="623" alt="Wreslting_Interface" src="https://github.com/user-attachments/assets/6164bd2c-8563-436d-9bd5-2dca55b3ed9c" />



## Agent GUI showing a weather forecast for Next PPV

<img width="796" height="623" alt="PPV_weather_looking_like" src="https://github.com/user-attachments/assets/8948654b-f270-4e2a-9157-b0ddd09474b0" />


<img width="802" height="599" alt="PPV-prt2" src="https://github.com/user-attachments/assets/30151a48-93e7-4279-b91a-a1474d4b881b" />


## Agent GUI answering wrestling trivia
<img width="1439" height="581" alt="triva_on_cena_punk" src="https://github.com/user-attachments/assets/fca40e14-20df-4c75-b9c7-a2156f590129" />

## The agent utilizing live web search to break down a historic championship rivalry.
<img width="1440" height="794" alt="final_shot" src="https://github.com/user-attachments/assets/2ff29a94-440d-463d-908c-85b2a1286321" />
<img width="1440" height="795" alt="final_shot_2" src="https://github.com/user-attachments/assets/0c11dd5d-6794-4b4f-bae1-67a2a1204a4d" />

## 🚀 Setup & Installation

1. **Clone the repository and install dependencies:**
   This project uses `uv` for lightning-fast dependency management.
   ```shell
   # Using pip
   pip install uv

2. **Configure your API Keys:**
Create a .env file in the root directory and add your personal keys. (Note: Never commit your .env file to GitHub!)

OPENAI_API_KEY=your_openai_api_key
SERPAPI_API_KEY=your_serpapi_api_key
MODEL_NAME=gpt-4o

3. **Launch the GUI:**

uv run wreslting.py
