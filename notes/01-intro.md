# Part 2: LLM Agent (Continued)
↴
## Context↴
- This is the second sharing in the series↴
- Part 1 covered: How to develop an LLM agent↴
- Retrospect: some audience confused LLM chatbot with LLM agent↴
- Need to clarify the distinction first before going deeper↴
↴
## Chatbot vs Agent — Key Distinction↴
↴
### LLM Chatbot↴
- The LLM chat API only responds once per message you send↴
- It can only answer your question — one turn at a time↴
- The **user** drives the conversation↴
↴
### LLM Agent↴
- The core idea: **who drives the conversation?**↴
- An agent drives the chat messages forward by itself — deciding what to do next, calling tools, observing results, and continuing↴
- It keeps pushing until it hits the goal↴
- The **agent** drives the conversation, not the user↴
↴
## The Key Insight↴
- Chatbot: user sends message → LLM responds → done (user-driven)↴
- Agent: user sets a goal → agent loops (think → act → observe) until goal is reached (agent-driven)↴
- The whole agent idea is about **how and who should drive the messages to push toward the goal**↴
