# 🚀 WhatsApp Conversational Voice AI Assistant

> Conversational AI Voice Assistant deployed on WhatsApp Business Cloud API with OpenAI Whisper STT, GPT-4o-mini, and ElevenLabs TTS.

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Security Policy](https://img.shields.io/badge/Security-Policy-success.svg)](SECURITY.md)
[![Ecosystem](https://img.shields.io/badge/Portfolio%20Ecosystem-341%20Studios-6366f1.svg)](https://pradeeptalari.me/projects/)
[![Architecture DAG](https://img.shields.io/badge/Architecture-DAG%20%26%20Course-10b981.svg)](https://pradeeptalari.me/tools/repo-learning/)
[![Flagship System](https://img.shields.io/badge/Flagship%20Platform-Production-0ea5e9.svg)](https://pradeeptalari.me/projects/whatsapp-voice-ai-assistant.html)

---

## 🏗️ System Architecture Flow

```mermaid
graph TD
    Client[Production Ingress / API Gateway] --> Router[Load Balancer & Route Controller]
    Router --> Engine[WhatsApp Conversational Voice AI Assistant Engine]
    Engine --> Storage[State & Cache Store: Redis / Vector DB]
    Engine --> Telemetry[OpenTelemetry Collector & SIEM]
    Telemetry --> SRE[Grafana Alertmanager & Incident SRE]
```

---

## 🚀 Step-by-Step Onboarding & Deployment Runbook

### 1. Prerequisites
- Docker & Docker Compose
- Python 3.10+ or Node.js runtime
- GitHub CLI (`gh`) & Git CLI

### 2. Clone Repository
```bash
git clone https://github.com/Pradeeptalari14/whatsapp-voice-ai-assistant.git
cd whatsapp-voice-ai-assistant
```

### 3. Configure Environment Variables
```bash
cp .env.example .env
# Edit .env with your environment parameters
```

### 4. Install Dependencies & Validate
```bash
bash scripts/validate.sh
```

### 5. Run Execution Engine
```bash
# Docker Run
docker build -t whatsapp-voice-ai-assistant:latest .
docker run --rm whatsapp-voice-ai-assistant:latest
```

---

## 🛡️ DevSecOps & Governance Standards

This repository follows standard production repository governance:
- **Security Scans**: Pre-commit hooks for Gitleaks, ShellCheck, and YAML validation.
- **Vulnerability Disclosure**: Strict vulnerability reporting process via [SECURITY.md](SECURITY.md).
- **Contributing Guidelines**: Conventional commits and review standards documented in [.github/CONTRIBUTING.md](.github/CONTRIBUTING.md).

---

*Synchronized with [WhatsApp Conversational Voice AI Assistant](https://pradeeptalari.me/projects/whatsapp-voice-ai-assistant.html) — [Talari Pradeep Portfolio](https://pradeeptalari.me)*
