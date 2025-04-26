# My First AI Agent

This is a simple AI agent using Google ADK (Agent Development Kit) to answer questions about weather and time in a specific city.

Repository: [https://github.com/fotsoeddy/My-First-AI-Agent-.git](https://github.com/fotsoeddy/My-First-AI-Agent-.git)

---

## Project Structure

```
my_agent_adk/
├── agent.py          # Main agent code
├── __init__.py
├── __pycache__/
├── requirements.txt  # Python dependencies
├── venv/             # Virtual environment (not included in repo)
```

## How to Setup and Run

1. **Clone the repository**

```bash
git clone https://github.com/fotsoeddy/My-First-AI-Agent-.git
cd My-First-AI-Agent-
```

2. **Create and activate a virtual environment**

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install the dependencies**

```bash
pip install -r requirements.txt
```

4. **Set up your environment variables**

Create a `.env` file in the root directory. Example:

```env
# .env file
GOOGLE_GENAI_USE_VERTEXAI=FALSE
GOOGLE_API_KEY=your-api-key-here
```

You can copy it from `.env.example`.

**If you are using Google AI Studio**, set `GOOGLE_GENAI_USE_VERTEXAI=FALSE` and add your API key from AI Studio.

**If you are using Vertex AI**, set:

```env
GOOGLE_GENAI_USE_VERTEXAI=TRUE
GOOGLE_PROJECT_ID=your-gcp-project-id
GOOGLE_LOCATION=your-vertexai-region
```

And ensure your environment has credentials:
```bash
export GOOGLE_APPLICATION_CREDENTIALS=/path/to/your/service-account-key.json
```

5. **Run the agent locally**

```bash
adk web
```

This will start a FastAPI web server where you can interact with your agent!

---

## What This Agent Can Do

- **Get Weather**: For example, "What is the weather like in New York?"
- **Get Time**: For example, "What time is it in New York?"

The agent uses simple hardcoded responses but is set up to extend easily.

---

## Contribution
Pull requests are welcome! Feel free to open issues to propose improvements or ask questions.


## License
This project is open-source and free to use. (You can add a LICENSE file if needed.)

---

**Made with ❤️ using Google ADK**

