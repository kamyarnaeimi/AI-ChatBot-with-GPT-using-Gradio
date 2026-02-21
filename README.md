# AI-ChatBot-with-GPT-using-Gradio
This project is a simple web-based chatbot interface built with Gradio and LangChain/OpenAI API. The chatbot can respond based on a role you define, so its answers are contextualized according to the role you assign.

# Features
Chat with GPT models (gpt-4o, gpt-4o-mini) via a simple Gradio interface.

Assign a role to the AI to shape its responses (e.g., business consultant, teacher, fitness coach).

Keep conversation history across multiple messages.

Easy to modify system prompts to change AI behavior.

Runs locally and can be deployed on a server.

# Installation
1. Clone the repository:
git clone https://github.com/yourusername/ai-chatbot-gradio.git
cd ai-chatbot-gradio

2. Create a virtual environment (recommended):
python -m venv venv
source venv/bin/activate  # Linux / Mac
venv\Scripts\activate     # Windows

3. Install dependencies:
pip install gradio langchain-openai

# Setup
1. Set your API key for the OpenAI-compatible endpoint
2. Choose the model you want to use
3. Optionally, change the system role

# How Roles Work
The system prompt defines the AI's role.

You can change the role to anything like:

"Business Analyst"

"Fitness Coach"

"Marketing Expert"

"Language Teacher"
Example: 
messages = [
    {"role": "system", "content": "You are a marketing expert. Give practical examples in marketing."}
]
# Folder Structure
ai-chatbot-gradio/
│
├─ app.py          # Main Gradio application
├─ requirements.txt
└─ README.md
