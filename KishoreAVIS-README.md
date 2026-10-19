# KishoreAVIS

**A personal agentic AI assistant that goes beyond a chatbot.**

KishoreAVIS is designed to understand natural-language and voice instructions, plan multi-step tasks, pick the right tools, and remember what matters over the long term.

> **Status:** Ongoing project, under active development.

---

## Goal

Build a personal AI assistant that can *do things*, not only answer questions: understand a request by text or voice, break it into steps, choose and call tools, use my own knowledge, and improve with memory over time.

## Capabilities and current status

| Capability | What it does | Status |
|---|---|---|
| Natural-language and voice input | Speech-to-text and text-to-speech with Whisper | Planned |
| Multi-step task planning | Breaks a goal into steps and executes them | Planned |
| Tool selection via function calling | Chooses the right tool for each step | Planned |
| Long-term semantic memory | Embeddings stored in a vector database | Planned |
| RAG | Answers grounded in my own documents and data | Planned |
| Multimodal input | Handles more than text | Planned |

*Status values: Working, In progress, Planned. Only mark something Working if it runs today.*

## Long-term vision

A central **orchestrator** that coordinates specialised agents:

| Agent | Purpose |
|---|---|
| Research | Find and summarise information |
| Coding | Help write and debug code |
| Productivity | Plan, schedule and organise |
| Knowledge | Answer from personal documents (RAG) |
| Automation | Carry out repetitive tasks |
| Wellness | Connect with wellness insights (see AURA) |

## Architecture (planned)

```
User (text / voice / image)
        |
   Orchestrator  <-->  Long-term memory (embeddings + vector DB)
     |    |    |
 Research Coding Productivity ...  <-->  Tools (function calling), RAG
```

## Tech stack

Python, FastAPI, Hugging Face, Whisper, vector databases, Docker, GitHub Actions

## Roadmap

- [ ] Core agent loop (plan, choose tool, act, observe)
- [ ] Function-calling tool set
- [ ] Voice input and output with Whisper
- [ ] Long-term memory with a vector DB
- [ ] RAG over personal documents
- [ ] Multimodal input
- [ ] Specialised agents and orchestrator
- [ ] Dockerised deployment with CI via GitHub Actions

## Getting started

```bash
git clone https://github.com/<your-username>/KishoreAVIS.git
cd KishoreAVIS
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
```

## Author

**Kishore Tambi Suddapalli**, MSc Artificial Intelligence student, Switzerland.
