# My First AI Agent

This project is called **my_agent_adk**, and it contains a simple AI agent built using [Google's AI Development Kit (ADK)](https://cloud.google.com/vertex-ai/docs/agents/overview). It is designed to answer user questions about **the weather** and **the current time** in a specific city.

---

## 📅 Project Structure

```bash
my_agent_adk/
├── agent.py           # Main agent definition and logic
├── __init__.py        # Makes this folder a Python package
├── __pycache__/       # Compiled Python cache files (auto-generated)
├── requirements.txt   # List of all dependencies
├── venv/              # Python virtual environment (recommended to use)
```

---

## 📦 Installation and Setup

First, clone the repository:

```bash
git clone https://github.com/fotsoeddy/My-First-AI-Agent-.git
cd My-First-AI-Agent-/my_agent_adk
```

Create and activate a virtual environment (optional but recommended):

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Make sure you have a `.env` file (you might need one depending on your ADK setup).

---

## 🧑‍💻 Running the Agent

To run the agent locally inside the ADK UI:

```bash
adk web ui --path=my_agent_adk/agent.py
```

Then open your browser at:

```bash
http://localhost:8080
```

You can interact with the agent using natural language. Example questions:
- "What's the weather like in New York?"
- "What time is it in New York?"

---

## 📈 Project Description

**My First AI Agent** is a simple but functional demonstration of how to build an AI agent using Google's ADK (AI Development Kit). It features two main tools:
- **get_weather**: Fetches static weather information for New York.
- **get_current_time**: Fetches the current time in New York based on timezone data.

It can be easily extended to add more cities, more services, or more tools for your custom needs.

---

## 📊 Tech Stack
- Python 3.12+
- [Google ADK](https://pypi.org/project/google-adk/)
- FastAPI
- Websockets

---

## 🛍️ License

This project is under the [MIT License](LICENSE) (you can add a LICENSE file if you wish).

---

## 🚀 Future Improvements
- Support weather and time for more cities
- Add real API integrations (like OpenWeatherMap)
- Enhance error handling and user prompts

---

> Made with ❤️ by [Eddy](https://github.com/fotsoeddy)

