# Agent Company OS

Your AI-powered executive assistant. Run entirely on your computer.

## 🎯 Vision

Build the ultimate personal AI company operating system - a beautiful, powerful desktop application that runs 100% locally on your computer, where you are the CEO and AI agents are your employees. No cloud dependencies. No data leaving your machine. Complete control. Infinite customization.

## ✨ Features

### CEO Dashboard
- Executive-style interface showing company health, team status, and projects
- Real-time agent activity monitoring
- Task delegation and tracking
- Performance analytics

### AI Employee Management
- Hire unlimited AI agents with custom roles
- 6 pre-built role templates (Research, Development, Content, Operations, Finance, Support)
- Extensive personality customization with sliders
- Visual avatar selection
- Capability and permission configuration

### Sandboxed Learning
- Safe training environment with mock data
- Structured training modules
- Skill assessments and certifications
- Continuous learning system

### Local-First AI
- Support for all local LLM providers:
  - Ollama (bundled)
  - LM Studio
  - LocalAI
  - KoboldCPP
  - vLLM
  - text-generation-webui
  - And more...
- Automatic provider discovery
- Model fallback chains
- No internet required

### Privacy & Security
- All data stored locally
- AES-256 encryption at rest
- Password/biometric authentication
- Zero telemetry by default
- Encrypted backups

## 🛠️ Tech Stack

### Frontend
- **Framework**: React 18 + TypeScript
- **UI**: shadcn/ui + Radix UI
- **Styling**: Tailwind CSS
- **State**: Zustand + TanStack Query
- **Routing**: React Router v6

### Backend (Rust)
- **Desktop**: Tauri
- **Database**: SQLite (SQLCipher encrypted)
- **Vector Store**: ChromaDB
- **AI Runtime**: Python + FastAPI

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- Rust 1.70+
- npm or pnpm

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-org/agent-company-os.git
   cd agent-company-os
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Install Tauri CLI**
   ```bash
   npm install -g @tauri-apps/cli
   ```

4. **Run in development**
   ```bash
   npm run tauri:dev
   ```

5. **Build for production**
   ```bash
   npm run tauri:build
   ```

## 📁 Project Structure

```
agent-company-os/
├── src-tauri/              # Rust backend
│   ├── src/
│   │   ├── main.rs         # Entry point
│   │   ├── agent_runtime/  # Agent execution
│   │   ├── model_provider/ # LLM integration
│   │   ├── storage/        # Local database
│   │   └── security/       # Encryption & auth
│   └── Cargo.toml
├── src/renderer/           # React frontend
│   └── src/
│       ├── components/     # UI components
│       ├── stores/         # State management
│       ├── types/          # TypeScript types
│       └── styles/         # CSS
├── resources/              # App resources
└── package.json
```

## 📋 Roadmap

### v0.1 - Alpha 
- [x] Project structure
- [x] Basic UI components
- [x] Agent CRUD operations
- [x] Dashboard layout
- [x] Ollama integration
- [x] Task execution

### v0.2 - Beta
- [x] Multiple agent roles
- [x] Training sandbox
- [x] Memory system
- [x] Model management UI

### v0.3 - Public Beta (current)
- [x] Complete CEO dashboard
- [x] Performance analytics
- [x] Backup & restore
- [x] Documentation

### v1.0 - General Availability
- [ ] All features complete
- [ ] Security audit
- [ ] App store submissions

## 🔒 Security

- All data encrypted with AES-256-GCM
- Password hashing with Argon2
- Sandboxed agent execution
- Resource limits enforced
- Network access controlled

## 📄 License

Proprietary - All rights reserved

## 🤝 Contributing

This is a commercial project. For partnership inquiries, contact: coming soon

## 💬 Support

- Documentation: [Coming Soon]
- Issues: GitHub Issues
- Discord: [Coming Soon]

---

**Agent Company OS** - Your AI employees. Your computer. Your data.
