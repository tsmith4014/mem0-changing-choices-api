<p align="center">
  <img src="logo.png" width="200" alt="Changing Choices Logo" />
</p>

# Changing Choices Memory API

**State-of-the-art memory for AI agents**  
Multi-session, graph-based, and long-term memory built for coaching, therapy, clinical, and custom LLM applications.

OpenMemory Memory Control Plane – modular, scalable, and privacy-first.  
Supports secure deployment (local or cloud) with Docker, Redis, and Postgres.

---

## About

Changing Choices Memory API powers the next generation of AI agent applications—especially in coaching, behavioral health, and problem gambling recovery.

- **Multi-session memory** for personalized client journeys  
- **Graph and long-term context** for smarter, more relevant AI  
- **Granular session privacy & isolation**  
- **Production-ready:** Docker, Redis, Postgres  
- **API-first** for easy integration into any AI agent, tool, or SaaS  
- **Perfect for:**  
  - AI coaching and therapy  
  - Clinical/research LLM tools  
  - Custom business, B2B, and compliance use cases

---

## Why Changing Choices Memory?

Traditional LLMs and chatbots forget everything after each session.  
Changing Choices Memory API enables persistent, structured, and explainable memory—letting your AI agent truly know its users and adapt over time, across sessions, and within strict privacy boundaries.

---

## Usage Example

```python
from mem0 import MemoryClient

client = MemoryClient(api_key="YOUR_API_KEY")
client.add(user_id, session_id, "User message...", meta={"context": "therapy"})
memories = client.get_all(user_id, session_id)
