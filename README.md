# Agentic AI Projects for Learning 🤖

Welcome to my repository for exploring **Agentic AI** workflows. This project focuses on building autonomous agents that can reason, use tools, and solve specific tasks dynamically.

The first project in this collection is a **Weather Agent** that demonstrates how an LLM can interact with real-world APIs to provide live data.

---

## 📋 Table of Contents
1. [About the Project](#-about-the-project)
2. [Project Structure](#-project-structure)
3. [Prerequisites](#-prerequisites)
4. [Setup Instructions](#-setup-instructions)
5. [How to Run](#-how-to-run)
6. [Security & API Keys](#-security--api-keys)
7. [Future Roadmap](#-future-roadmap)

---

## 🌟 About the Project
Unlike standard chatbots, this **Weather Agent** uses a ReAct (Reason + Act) pattern. It doesn't just guess the weather; it identifies that it needs a tool, calls a weather API, and processes the raw JSON into a human-readable response.



---

## 📂 Project Structure
```text
Agentic-AI-Projects-for-learning/
├── weatheragent/         # Core logic for the weather agent
│   └── agent.py          # Execution script
├── .env.example          # Template for required API keys
├── .gitignore            # Keeps venv and secrets out of GitHub
├── README.md             # Project documentation
└── requirements.txt      # Python dependencies

## 🛠️ Setup Instructions
1. Clone the Repository
Bash
git clone [https://github.com/Gaurav-Dongare/Agentic-AI-Projects-for-learning.git](https://github.com/Gaurav-Dongare/Agentic-AI-Projects-for-learning.git)
cd Agentic-AI-Projects-for-learning
2. Create and Activate Virtual Environment
Keeping your global Python installation clean is best practice.

Bash
# Create the environment
python -m venv venv

# Activate it (Windows)
venv\Scripts\activate

# Activate it (Mac/Linux)
source venv/bin/activate

3. Install Dependencies
Bash
pip install -r requirements.txt
🔑 Security & API Keys
This project uses a .env file to manage sensitive information. Never upload your actual .env file to GitHub.

Locate the .env.example file in the root directory.

Create a copy and rename it to .env:

Bash
cp .env.example .env
Open .env and add your specific API keys:

Plaintext
OPENAI_API_KEY=your_openai_key_here
WEATHER_API_KEY=your_weather_api_key_here
🚀 How to Run
Once your environment is active and keys are configured, start the agent by running:

Bash
python weatheragent/agent.py
🗺️ Future Roadmap
[ ] CNC Monitoring: Integrate Fanuc FOCAS for real-time production tracking.

[ ] Web Interface: Add a FastAPI or Streamlit frontend.

[ ] Multi-Agent Systems: Enable multiple agents to collaborate on complex engineering tasks.

👤 Author
Gaurav Dongare
Mechanical Engineer & AI Enthusiast
GitHub Profile


---

### A quick tip for your `.env.example`:
To make this work perfectly for others, create a file named `.env.example` in your folder and just put this inside:

```text
# Replace the placeholders with your actual keys
OPENAI_API_KEY=your_openai_api_key_here
WEATHER_API_KEY=your_weather_api_key_here
