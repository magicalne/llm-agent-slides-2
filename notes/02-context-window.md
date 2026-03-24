# Context Window: 1M Tokens — Reality Check
↴
## The Claim↴
- Gemini, OpenAI, Anthropic all claim ~1M token context window↴
- Xiaomi's new model also claims 1M context↴
- But claiming support ≠ actually being able to use it effectively↴
↴
## Needle in a Haystack Benchmark↴
- A benchmark that tests whether an LLM can retrieve a specific piece of information (the "needle") buried inside a massive amount of irrelevant text (the "haystack")↴
- You hide a small fact deep in a huge context, then ask the model to find it↴
- Tests whether the model truly attends to the full context or just the beginning/end↴
↴
## The Reality↴
- AFAIK, only Claude Opus 4.6 handles the full 1M context for real↴
- Other models degrade significantly as context grows — they lose track of information in the middle↴
- If you're stuffing 1M tokens into GPT-5.4, you're throwing money into a hole↴
- The model can't reliably use all that context, so you're paying for tokens that don't help
## Why This Matters for Agents↴
- Agents accumulate context over many turns (tool calls, observations, reasoning)↴
- If your model can't handle long context well, agent performance degrades over time↴
- Context management strategy matters — don't just blindly fill the window↴
