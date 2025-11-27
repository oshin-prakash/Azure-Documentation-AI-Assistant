# Azure-Documentation-AI-Assistant
A Python project that integrates Azure AI Agents with the Microsoft Learn MCP server. It creates on-demand agents capable of searching official Microsoft documentation and responding with tool-enhanced reasoning.

**🚀 Features**

Azure AI Agent Integration
Creates and orchestrates Azure AI agents using the official SDK.

MCP (Model Context Protocol) Support
Connects to the Microsoft Learn MCP server for real-time doc search.

Interactive Chat Flow
Accepts user input from the terminal and routes it to the agent.

Run & Tool Call Logging
Prints step-by-step execution details, MCP tool calls, and run status.

Environment Configuration
Uses a .env file to securely store credentials and endpoints.

Automatic Cleanup
Deletes the agent after the session to keep your environment clean.

**🧭 Architecture Overview**

┌─────────────────────┐
│      User Input      │
└───────────┬─────────┘
            │
            ▼
┌─────────────────────┐        ┌──────────────────────────┐
│ Azure AI Agent SDK  │◄──────►│ Microsoft Learn MCP Tool │
└─────────────────────┘        └──────────────────────────┘
            │
            ▼
┌─────────────────────┐
│     AI Response      │
└─────────────────────┘

**📁 Project Structure**

azure-mcp-agent/
│
├── src/
│   ├── main.py
│   ├── mcp_config.py
│   └── utils.py
│
├── .env.example
├── requirements.txt
├── README.md
└── .gitignore

**🔧 Setup**

1. Clone the repository
git clone https://github.com/yourusername/azure-mcp-agent.git
cd azure-mcp-agent

2. Install dependencies
pip install -r requirements.txt

3. Configure environment variables

Rename .env.example → .env and fill:

PROJECT_ENDPOINT=your_azure_ai_endpoint
MODEL_DEPLOYMENT_NAME=your_model

4. Run the project
python src/main.py

**📝 Use Cases**

🔍 Search Microsoft documentation using natural language

🤖 Build smart agents that can browse docs while thinking

🧪 Experiment with MCP inside Azure AI Agents

🛠️ Create your own tool-enabled agent system

🎓 Learning and teaching Azure + MCP integrations

**🧪 Requirements
**
Python 3.9+

Azure subscription with AI Agents enabled

Microsoft Learn MCP server access

Azure CLI / VS Code logged-in identity


