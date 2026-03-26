 Plugex-Code
AI Coding Assistant with Guardrails & Multi-Agent System

<img width="329" height="93" alt="image" src="https://github.com/user-attachments/assets/baf45912-bb85-471a-9d4d-5ba7106a88e9" />







🎯 Overview
Plugex-Code is a privacy-first, local-first AI coding assistant that runs 100% on your machine. It features:
·	Glass Box Visibility - See AI reasoning before any code changes
·	100-Agent System - Create specialized agents for any task
·	KillPlug Security - Real-time security scanning and guardrails
·	Natural Language Interface - Just ask what you want in plain English
·	Autonomous Debugging - Self-correcting code generation
·	Multi-Model Support - Works with Ollama, LM Studio, and more

🚀 Quick Install
One-Line Install (Recommended)
# Using curl
curl -fsSL https://raw.githubusercontent.com/YOUR_GITHUB_USERNAME/Plugex-Code/main/install.sh | bash

# Or using wget
wget -qO- https://raw.githubusercontent.com/YOUR_GITHUB_USERNAME/Plugex-Code/main/install.sh | bash

Manual Install
# 1. Clone the repository
git clone https://github.com/YOUR_GITHUB_USERNAME/Plugex-Code.git ~/Plugex-Code
cd ~/Plugex-Code

# 2. Run the installer
./install.sh

# 3. Add to PATH (if not already done)
export PATH="$HOME/.local/bin:$PATH"

Requirements
·	Python 3.10+
·	pip and python3-venv
·	Git (optional, for cloning)
·	Ollama (optional, for local LLM)
Install dependencies on Ubuntu/Debian:
sudo apt update && sudo apt install python3 python3-pip python3-venv git


🎮 Usage
Start Interactive Chat
# Default (uses configured model)
Plugex-Code

# With specific provider
Plugex-Code --provider ollama --model qwen 3.5:9b

# With LM Studio
Plugex-Code --provider LM Studio --model gemma:9B

# Single message mode
Plugex-Code --message "Create a Python function that sorts a list"

Natural Language Commands
Just ask in plain English:
create a frontend developer agent
create a python expert named py_helper
list all agents
write a Python script that calculates fibonacci numbers
create a file called config.json with database settings
delete the test.txt file
show me git status
explain how authentication works in this project

Agent Management
# Create specialized agents
create a backend engineer named api_master
create a security specialist called sec_guru
create a devops engineer
create a qa tester
create a tech lead to review code

# Create teams
create a web dev team
create a coding team with frontend and backend agents

# List and manage
list all agents
stop agent api_master
remove agent sec_guru


🛡️ KillPlug Security
Plugex-Code includes built-in security scanning:
·	Prompt Injection Detection - Blocks manipulation attempts
·	Hardcoded Secret Scanning - Finds API keys, passwords, tokens
·	Dangerous Command Blocking - Prevents harmful operations
·	Path Traversal Protection - Blocks unauthorized file access
·	Vulnerable Pattern Detection - Identifies security issues
Security levels:
·	strict - Maximum protection
·	balanced - Default (recommended)
·	permissive - Minimal protection
·	off - No scanning

🤖 Agent System
Available Agent Roles
Role	Expertise
Architect	System design, architecture patterns
Backend	Python, APIs, databases
Frontend	React, Vue, TypeScript, CSS
Fullstack	End-to-end development
DevOps	CI/CD, Docker, Kubernetes
QA	Testing, automation
Security	Vulnerability scanning
Reviewer	Code review, documentation
ML Engineer	Machine learning, PyTorch
Data Scientist	Analysis, pandas, visualization
Mobile Dev	iOS, Android, Flutter
Game Dev	Unity, Unreal, Godot
Database Admin	PostgreSQL, MySQL, MongoDB
Cloud Architect	AWS, GCP, Azure
And 40+ more specialized roles!	

Agent Capabilities
·	Auto-scaling - Up to 100 concurrent agents
·	Load balancing - Intelligent task distribution
·	Group support - Organize agents by function
·	Role-based selection - Best agent for each task

📁 Project Structure
Plugex-Code/
├── src/                    # Source code
│   ├── core/              # Engine, config, guardrails
│   ├── agents/            # Agent system (100 agents)
│   ├── cli/               # Command-line interface
│   ├── tools/             # Tool definitions
│   └── plugins/           # KillPlug security plugin
├── install.sh             # Installation script
├── requirements.txt       # Python dependencies
└── Plugex-Code           # Main executable


⚙️ Configuration
Create ~/.plugex/config.yaml:
llm:
  provider: ollama
  model: qwen2.5:7b
  cloud_fallback: false

security:
  level: balanced  # strict, balanced, permissive, off

glass_box:
  enabled: true
  show_reasoning: true

mentor_mode:
  enabled: false  # Get explanations while learning


🔧 Development
Run from Source
cd ~/Plugex-Code

# Create virtual environment
python3 -m venv .venv
source .venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run the CLI
python src/cli/chat_cli.py

Run Tests
pytest tests/


🆘 Troubleshooting
Command Not Found
# Add to PATH
export PATH="$HOME/.local/bin:$PATH"

# Add to ~/.bashrc for persistence
echo 'export PATH="$HOME/.local/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc

Model Not Available
# For Ollama, pull the model
ollama pull qwen 3.5:9B

# Or use a different provider
Plugex-Code --provider LM Studio -- Gemma:9B

Permission Denied
# Make executable
chmod +x ~/Plugex-Code/Plugex-Code
chmod +x ~/Plugex-Code/install.sh


📝 License
Custom License - See LICENSE file for details.

🙏 Acknowledgments
·	Built with ❤️ for the open-source community
·	Powered by local LLMs (Ollama, llama.cpp)
·	Security by KillPlug plugin architecture

📞 Support
·	Issues: GitHub Issues
·	Discussions: GitHub Discussions

Plugex-Code - Your AI pair programmer, running 100% locally. 🔌🚀
