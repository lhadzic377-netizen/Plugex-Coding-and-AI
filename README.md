<img width="329" height="93" alt="image" src="https://github.com/user-attachments/assets/7903db12-d15d-4e39-b64f-54bddbc99321" />
**Plugex Code & Plugex AI**  
**Privacy-First Local AI Coding Assistant**  
Plugex is a local-first AI coding platform that runs 100% on your machine. It combines the power of intelligent agents with revolutionary Knowledge Shard architecture for fast, context-aware coding assistance.  
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANUlEQVR4nO3OQQmAABRAsSdYxZ4/mJjEsxE8W8GbCFuCLTOzVXsAAPzFuVZ3dXw9AQDgtesBxPEF3bv7x0IAAAAASUVORK5CYII=)  
**Plugex Code**  
A transparent AI coding partner with glass-box visibility, autonomous debugging, and multi-agent orchestration.  
**Features**  
- **Glass Box Visibility** - See AI reasoning before code changes  
- **Multi-Agent System** - Create specialized agents (frontend, backend, security, QA)  
- **Agent Swarms** - Parallel task execution with coordinated agents  
- **Natural Language Interface** - Just say what you want  
- **Autonomous Debugging** - Self-correcting code generation  
- **Plugin Architecture** - Extensible security and utility plugins  
- **Local-First** - Runs on local models, privacy guaranteed  
**Quick Start**  
# Start interactive chat  
 codeplug  
   
 # Or with specific provider/model  
 codeplug --provider ollama --model qwen3.5:2b  
   
**Natural Language Commands**  
create a frontend developer agent  
 create a python expert named py_helper  
 list all agents  
 write a Python script that calculates fibonacci numbers  
 create a file called config.json  
 delete the file  
 show me git status  
   
**Agent System**  
# Create specialized agents  
 create a backend engineer named api_master  
 create a security specialist called sec_guru  
 create a devops engineer  
   
 # Create teams  
 create a web dev team  
 create a coding team with frontend and backend agents  
   
 # List and manage  
 list all agents  
   
**Slash Commands**  
| | |  
|-|-|  
| **Command** | **Description** |   
| /read <file> | Read file contents |   
| /write <file> | Create/write file |   
| /edit <file> | AI-assisted editing |   
| /debug <file> | Debug with auto-fix |   
| /run <cmd> | Execute shell command |   
| /agent | Manage agents |   
| /swarm | Agent swarm commands |   
| /team | Team management |   
| /clear | Clear chat history |   
| /help | Show all commands |   
   
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANElEQVR4nO3OQQmAABRAsad4EjtY9fewnUms4E2ELcGWmTmrKwAA/uLeqrU6vp4AAPDa/gDzWAM6QQXRdAAAAABJRU5ErkJggg==)  
**Plugex AI**  
A local RAG (Retrieval-Augmented Generation) system with revolutionary Knowledge Shard architecture.  
**Features**  
- **100% Local** - No cloud, no API keys, your data never leaves your machine  
- **Knowledge Shards** - Modular, loadable knowledge units (not one big slow database)  
- **Fast & Efficient** - Only load what you need, when you need it  
- **Multi-Model Support** - Qwen 3.5 family (0.8B to 397B parameters)  
- **Thinking Modes** - Fast mode for quick answers, Thinking mode for deep reasoning  
- **Source Attribution** - Every answer shows exactly where it came from  
- **Hardware Adaptive** - Automatically recommends best model for your system  
**Quick Start**  
# Start chatting  
 plugex-ai chat  
   
 # Index your codebase  
 plugex-ai index ./my-project  
   
 # Ask a question  
 plugex-ai query "How does authentication work in this codebase?"  
   
**Knowledge Shard Architecture**  
Unlike traditional RAG systems that load everything into memory, Plugex uses Knowledge Shards:  
~/.plugex/shards/  
 ├── core/                    # Always available  
 │   ├── algorithms           # Sorting, searching, data structures  
 │   ├── patterns             # Design patterns & best practices  
 │   └── errors               # Common errors & fixes  
 │  
 ├── languages/               # Load on demand  
 │   ├── python               # Python docs & examples  
 │   ├── javascript           # JavaScript/Node docs  
 │   └── rust                 # Rust documentation  
 │  
 ├── frameworks/              # Load on demand  
 │   ├── react                # React docs  
 │   ├── django               # Django docs  
 │   └── fastapi              # FastAPI docs  
 │  
 └── projects/                # Your codebases  
     ├── my-app               # Your indexed projects  
     └── work-project  
   
**Why Shards?**  
| | | |  
|-|-|-|  
| **Feature** | **Traditional RAG** | **Knowledge Shards** |   
| Memory Usage | 10GB+ always loaded | 50-200MB typical |   
| Load Time | Slow (minutes) | Instant |   
| Search Speed | Slower (searches all) | Faster (relevant shards only) |   
| Updates | Rebuild everything | Update single shard |   
| Scalability | Limited | Unlimited (1EB+ possible) |   
   
**Commands**  
***Chat***  
# Interactive chat  
 plugex-ai chat  
   
 # With specific model  
 plugex-ai chat --model qwen3.5:2b  
   
 # Fast mode (no thinking)  
 plugex-ai chat --fast  
   
 # Thinking mode (better reasoning)  
 plugex-ai chat --think  
   
In-chat commands:  
- /fast - Switch to fast mode  
- /think - Switch to thinking mode  
- /mode - Toggle between modes  
- /help - Show all commands  
- /quit - Exit chat  
***Index Documents***  
# Index your codebase  
 plugex-ai index ./my-project  
   
 # Index into specific shard  
 plugex-ai index ./python-lib --shard python-docs  
   
 # Recursive indexing (default)  
 plugex-ai index ./src --recursive  
   
***Query***  
# Single question  
 plugex-ai query "What does the auth function do?"  
   
 # With top-k results  
 plugex-ai query "Explain sorting algorithms" --top-k 10  
   
***Knowledge Shards***  
# List all shards  
 plugex-ai shard list  
   
 # Create a new shard  
 plugex-ai shard create my-project --category projects --languages python  
   
 # Load a shard into memory  
 plugex-ai shard load python-docs  
   
 # Unload a shard  
 plugex-ai shard unload python-docs  
   
 # Show shard info  
 plugex-ai shard info algorithms  
   
 # Show shard manager stats  
 plugex-ai shard stats  
   
 # Delete a shard  
 plugex-ai shard delete my-project  
   
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANklEQVR4nO3OMQ2AABAAsSPBCj5fFgpQwYwEZiywEZJWQZeZ2ao9AAD+4lyruzq+ngAA8Nr1AMTRBeEgNK9YAAAAAElFTkSuQmCC)  
**Supported Models**  
**Qwen 3.5 Model Family**  
| | | | |  
|-|-|-|-|  
| **Model** | **Size** | **RAM Required** | **Best For** |   
| 0.8B | 1.0GB | 2GB | Minimal systems |   
| 2B | 2.7GB | 4GB | Low-RAM systems |   
| 4B | 3.4GB | 6GB | Compact performance |   
| 8B | 6.6GB | 10GB | Best balance |   
| 27B | 17GB | 24GB | Complex reasoning |   
| 35B | 24GB | 32GB | Premium quality |   
| 122B | 81GB | 96GB | Flagship |   
| 397B | 240GB | 320GB | Ultra-flagship |   
   
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANElEQVR4nO3OQQmAABRAsad4EEtY9QcxnUms4E2ELcGWmTmrKwAA/uLeqrU6vp4AAPDa/gDzXgM37EF77AAAAABJRU5ErkJggg==)  
**Installation**  
**Requirements**  
- Python 3.10+  
- Ollama (for local LLM inference)  
- 4GB+ RAM (8GB+ recommended)  
**Quick Install**  
# Clone the repository  
 git clone https://github.com/dcbcable/plugex.git  
 cd plugex  
   
 # Run installer  
 ./install.sh  
   
 # Or manually link  
 ln -s $(pwd)/plugex ~/bin/plugex-ai  
   
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANklEQVR4nO3OQQmAABRAsSfYxZo/jVEMYQLPJrCCNxG2BFtmZquOAAD4i3Ot7mr/egIAwGvXA4rLBc059ysnAAAAAElFTkSuQmCC)  
**Configuration**  
Config stored in ~/.plugex/config.json:  
{  
   "model": "qwen3.5:2b",  
   "index_path": "/home/user/.plugex/index",  
   "thinking_mode": false  
 }  
   
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANUlEQVR4nO3OQQmAABRAsSfYxKK/kYXEkyk8WcGbCFuCLTOzVXsAAPzFuVZ3dXw9AQDgtesB/v8F8JQadPwAAAAASUVORK5CYII=)  
**Architecture**  
plugex/  
 ├── ai/  
 │   ├── shards/              # Knowledge Shard system  
 │   │   ├── shard.py         # Shard class  
 │   │   └── manager.py       # ShardManager with LRU  
 │   ├── rag/                 # RAG pipeline  
 │   │   ├── pipeline.py      # Main RAG logic  
 │   │   ├── llm.py           # LLM client  
 │   │   └── prompts.py       # Prompt templates  
 │   ├── vector_index/        # Vector search  
 │   ├── chunking/            # Document chunking  
 │   └── config/              # Hardware detection  
 ├── agents/                  # Multi-agent system  
 │   ├── base.py              # Agent base classes  
 │   ├── orchestrator.py      # Agent coordination  
 │   ├── swarm.py             # Parallel execution  
 │   └── teams.py             # Role-based teams  
 ├── core/                    # Core engine  
 │   ├── engine.py            # Main engine  
 │   ├── unified_tools.py     # Tool system  
 │   └── guardrails.py        # Safety system  
 ├── cli/                     # CLI interface  
 │   ├── chat_cli.py          # Interactive chat  
 │   └── main.py              # Command handler  
 └── plugex                   # Main CLI  
   
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANklEQVR4nO3OMQ2AABAAsSNBACPiUML0NpGACyywEZJWQZeZ2aszAAD+4l6rrTq+ngAA8Nr1AL/SBEZwuCSwAAAAAElFTkSuQmCC)  
**Examples**  
**Debug Your Code**  
plugex-ai chat  
   
 /think Why is my auth middleware failing?  
   
 [Plugex searches auth-related code in your project]  
 [Returns specific answer with file:line references]  
   
**Learn Algorithms**  
plugex-ai query "Explain quicksort with Python example"  
   
 [Plugex loads algorithms shard]  
 [Returns explanation + code example]  
   
**Code Review**  
plugex-ai index ./my-project --shard my-project  
 plugex-ai query "Review the user authentication flow" --shard my-project  
   
**Create Agents**  
create a frontend developer agent  
 create a backend engineer named api_master  
 list all agents  
   
 # Create a team for a project  
 create a web dev team  
   
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANUlEQVR4nO3OsQ1AABRAwSdRaPXGMOCv7WkPK+hEcjfBLTNzVFcAAPzFvVZbdX49AQDgtf0BSpoDXv5TGXgAAAAASUVORK5CYII=)  
**Query Flow**  
1. User asks: "How do I sort a list in Python?"  
    ↓  
 2. ShardManager detects:  
    - Language: python  
    - Topic: algorithm (sorting)  
    ↓  
 3. Auto-loads relevant shards:  
    - core/algorithms  
    - languages/python  
    ↓  
 4. Searches only those shards  
    ↓  
 5. Returns answer with sources  
   
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANklEQVR4nO3OQQmAABRAsSeYxZw/lVeDGMACBrCCNxG2BFtmZquOAAD4i3Ot7mr/egIAwGvXA6fOBdd+dKAKAAAAAElFTkSuQmCC)  
**Memory Management**  
- **Core shards** stay in memory while chat is active  
- **Language/Framework shards** load on demand, expire after TTL  
- **Project shards** load when working on that project  
- **LRU eviction** when max shards reached  
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANUlEQVR4nO3OQQmAABRAsSfYxKK/kYXEkyk8WcGbCFuCLTOzVXsAAPzFuVZ3dXw9AQDgtesB/v8F8JQadPwAAAAASUVORK5CYII=)  
**Security Features**  
- **Guardrails System** - Protection levels for file operations  
- **KillPlug Integration** - Security scanning for sensitive data  
- **Confirmation Prompts** - User approval for dangerous operations  
- **Backup System** - Automatic backups before modifications  
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAALUlEQVR4nO3OQQ0AIAwEsAMlSJ0UrOFkGngRklZBR1WtJDsAAPzizNcDAADuNcKwAyU+nb+5AAAAAElFTkSuQmCC)  
**Contributing**  
1. Fork the repository  
2. Create a feature branch  
3. Make your changes  
4. Submit a pull request  
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANElEQVR4nO3OQQmAUBBAwSfIb+HdmNvAkgaxgjcRZhLMNjNHdQUAwF/ce7Wq8+sJAACvrQctewNKtdojwQAAAABJRU5ErkJggg==)  
**License**  
Custom License - See LICENSE file  
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAnEAAAACCAYAAAA3pIp+AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAA7EAAAOxAGVKw4bAAAANUlEQVR4nO3OMQ2AABAAsSNhwgJuUPYDMpnRgQU2QtIq6DIze3UGAMBf3Gu1VcfXEwAAXrseaHEEM+cJoFcAAAAASUVORK5CYII=)  
**Acknowledgments**  
- Built with Ollama for local LLM inference  
- Uses Qwen models by Alibaba Cloud  
- Inspired by RAG research from Meta, Google, and OpenAI  
