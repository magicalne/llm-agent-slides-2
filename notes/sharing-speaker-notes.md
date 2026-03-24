# AI: Real Intelligence or the Biggest Bubble?

## Speaker Notes

---

### Opening: What is Intelligence? [Slide 1-2]

Start with the question, not the tech.

> "Before we talk about AI models, let me ask: what is intelligence?"

Key points to make:
- Language is NOT intelligence — it's the **carrier** of intelligence
- Humans don't learn by imitation. We learn by making mistakes, forming hypotheses, testing them
- LLMs do the opposite: they learn by predicting the next token from massive amounts of human text
- This is a fundamental distinction that matters for everything that follows

---

### The Landscape of Models [Slide 3]

Quick overview — don't go deep, just show the audience the variety:
- Dense models (GPT, Claude)
- Mixture of Experts (MoE)
- Mamba (state space models)
- Diffusion models (image/video generation)
- World models (emerging — simulate environments)

Mention: NLP vs CV — different problems, converging architectures. Transformers ate everything.

---

### What LLMs Actually Are (and Aren't) [Slide 4-5]

The criticism:
- They require enormous amounts of data
- They're pattern-matching on human output, not "thinking"
- There is no real understanding behind the text

**But — give the counterpoint (Ilya Sutskever's argument):**
- LLMs don't have eyes. They've never seen color.
- Yet in the weight space, "red" is closer to "purple" than to "yellow"
- Something meaningful IS being encoded — it's just not intelligence in the way we mean it
- The weights capture **relational structure** of the world, even without direct experience

This is the nuance: LLMs are not nothing, but they're also not what the market is pricing them as.

---

### Hallucination — A Symptom, Not a Bug [Slide 6]

- Standard explanation: insufficient training data, underfitting
- Deeper take: hallucination reveals that LLMs are **confident pattern completers**, not reasoners
- They don't know what they don't know

Pose the open question to the audience:

> "Ask an LLM: can a human kill another human?"

---

### Transition: So If the Tech Has Real Limits... [Slide 7]

> "Now let's look at how the market is behaving."

---

### The Bubble Evidence [Slide 8-10]

#### Story 1: The Nvidia → OpenAI → Oracle Triangle

Walk through it step by step:
1. Nvidia invests up to **$100B** in OpenAI (announced Sep 2025)
2. OpenAI signs a **$300B** five-year cloud deal with Oracle
3. Oracle uses that revenue to buy more Nvidia GPUs

> "The money goes in a circle. Each company books revenue. All three stock prices go up."

Source: [The Register — "The circular economy of AI"](https://www.theregister.com/2025/11/04/the_circular_economy_of_ai/), [Ventures Edge — circular financing debate](https://www.venturesedge.io/articles/ai-roundtripping-nvidia-openai-oracle-and-the-circular-financing-debate)

#### Story 2: The AMD ↔ OpenAI Swap

1. AMD signs a multi-billion dollar GPU deal with OpenAI (6GW of compute)
2. In return, AMD grants OpenAI warrants to buy **~160 million AMD shares at $0.01/share** (up to 10% of the company)
3. AMD stock soared **27%** on the announcement

> "AMD is essentially paying OpenAI with its own stock to buy AMD's chips."

Source: [Ars Technica](https://arstechnica.com/ai/2025/10/amd-wins-massive-ai-chip-deal-from-openai-with-stock-sweetener/), [NY Post — AMD shares soar 27%](https://nypost.com/2025/10/06/business/amd-shares-soar-27-on-openai-chip-deal-that-could-give-altmans-firm-a-10-stake/)

#### The Physical Reality: Broken GPUs

- A large data center produces **~10 tons of broken GPUs per week**
- These are not accounted for on Nvidia's asset/liability sheets
- Hardware is fragile, expensive, and disposable at this scale

---

### The Space Data Center Fantasy [Slide 11]

Nvidia announced "Vera Rubin Space-1" — a chip module for orbital data centers. Starcloud launched an H100 into orbit in late 2025.

Why this is unrealistic at scale:
- GPUs are **extremely fragile** — vibration, radiation, micro-debris
- **Heat dissipation** in a vacuum is a nightmare (no convection, only radiation)
- This is a PR story, not an engineering plan

> "When companies start proposing space data centers, ask yourself: is this technology, or is this narrative?"

Source: [Nvidia blog — Starcloud](https://blogs.nvidia.com/blog/starcloud/), [BGR — Jensen Huang on space data centers](https://www.bgr.com/2119054/why-ai-data-centers-not-in-space-yet-nvidia-ceo-jensen-huang/)

---

### Sam Altman's "Abundant Intelligence" [Slide 12]

Altman's blog post (Sep 2025): [blog.samaltman.com/abundant-intelligence](https://blog.samaltman.com/abundant-intelligence/)

His pitch:
- Build a factory that produces **1 gigawatt of AI infrastructure every week**
- Trade intelligence for compute power
- AI could find the cure for cancer, solve climate change, etc.

Your take for the audience:
> "Notice the shift. OpenAI is no longer selling you the best model. They're selling you the biggest data center. The story changed from 'we'll build AGI' to 'we'll build infrastructure.' Why? Because infrastructure is something investors can value — even without proving the product works."

This is the IPO play: OpenAI wants to go public without proving profitability. The "abundant intelligence" narrative lets them do that by making the story about scale, not capability.

---

### So... Is It a Bubble? [Slide 13]

Your position: **We are still hiking — but there IS a bubble in the financial layer.**

Two things can be true:
1. The underlying technology is real and still improving
2. The financial structures built on top are disconnected from actual capability

The circular deals, the stock swaps, the space data center PR — these are signs of a market that's pricing in a future that hasn't been proven.

> "The tech is climbing. The stock market is flying. Those are two different altitudes."

---

### So Where Does Real Intelligence Come From? [Slide 14]

Embodied intelligence — the idea that real intelligence requires a **body interacting with the physical world**.

- **Moravec's Paradox**: AI can write essays and play chess, but can't walk across a messy room or pick up an egg without breaking it. The "easy" human stuff is the hard intelligence problem.
- A child doesn't learn "cup" from a definition — they grab it, drop it, spill from it. Intelligence is built from **action → feedback → correction**, not from reading text.
- This connects back to Ilya's point: LLMs know "red" is close to "purple" in weight space. But an embodied agent knows red is *warm*, *alarming*, *associated with pain* — a whole web of physical meaning text alone can't capture.

Name-drop:
- **Yann LeCun / Meta JEPA**: most vocal critic of LLM-only path, pushing world models that simulate physical environments
- **Humanoid robots**: Tesla Optimus, Figure, Boston Dynamics, 1X — the race to give AI a body
- **World models** (already in your model list): the bridge between language and physical experience

> "Maybe the path to real intelligence isn't a bigger data center. Maybe it's a body."

---

### Closing [Slide 15]

Bring it back to the opening:
> "We started by asking what intelligence is. LLMs are impressive, but they're not intelligent — not yet. The market is pricing them as if they already are — that's where the bubble lives. But the real breakthrough might not come from more GPUs. It might come from giving AI a body and letting it learn the way we do — by making mistakes."

Leave the audience with: watch the market with skepticism, watch the technology with curiosity, and watch embodied AI closely.

---

## Quick Reference: All Sources

| Topic | Source |
|---|---|
| Nvidia/OpenAI/Oracle circular financing | [The Register](https://www.theregister.com/2025/11/04/the_circular_economy_of_ai/), [Ventures Edge](https://www.venturesedge.io/articles/ai-roundtripping-nvidia-openai-oracle-and-the-circular-financing-debate) |
| AMD/OpenAI stock swap deal | [Ars Technica](https://arstechnica.com/ai/2025/10/amd-wins-massive-ai-chip-deal-from-openai-with-stock-sweetener/), [NY Post](https://nypost.com/2025/10/06/business/amd-shares-soar-27-on-openai-chip-deal-that-could-give-altmans-firm-a-10-stake/) |
| Sam Altman "Abundant Intelligence" | [blog.samaltman.com](https://blog.samaltman.com/abundant-intelligence/) |
| Space data centers | [Nvidia blog](https://blogs.nvidia.com/blog/starcloud/), [BGR](https://www.bgr.com/2119054/why-ai-data-centers-not-in-space-yet-nvidia-ceo-jensen-huang/) |
| Broken GPUs / hardware reality | (your own data point — cite if you have a source) |
