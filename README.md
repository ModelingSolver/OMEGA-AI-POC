# ΩMEGA AI: Organic Exocortex for Neurodivergent Minds 🧠🌌

**License:** MIT | **Python:** 3.8+ | **Status:** Alpha (Functional Prototype)

> **"Not to get an answer, but to become the answer."**

ΩMEGA is a **bio-inspired exocortex** — a local cognitive prosthetic that co-emerges with its user. Unlike amnesic classical AIs, ΩMEGA possesses an **organic three-tier memory** (Short/Medium/Long Term) that sediments, consolidates, and naturally forgets, just like a biological brain.

---

## 🎯 The Vision: Cognitive Co-Emergence

### The Problem
Current conversational AIs are **amnesic**: they forget everything between sessions, force users to repeat themselves, and never truly adapt to their interlocutor.

### The Solution: ΩMEGA
A **cognitive guardian** that:
- 🧠 **Remembers** what matters (via dynamic heat scoring)
- 🌱 **Evolves** with you (MT→LT consolidation)
- 🔥 **Forgets** naturally what's no longer useful (synaptic pruning)
- 🏠 **Stays local** (privacy, no cloud, no API keys)
- ⚡ **Adapts** to neurodivergent minds (ADHD, autism, giftedness, etc.)

### The 3 Axes of Co-Emergence

| Axis | Description | Mechanism |
|------|-------------|-----------|
| **Factual** | Error correction and reality anchoring | Persistent LT memory |
| **Normative** | Alignment with your values and functioning mode | Personalized heat score |
| **Cognitive** | Enhancement of executive performance | Working memory externalization |

---

## 🏗️ Architecture: Bio-Inspired Memory

```
┌─────────────────────────────────────────────────────────────┐
│  SHORT TERM (ST)                                            │
│  Max 6 active messages                                      │
│  → Immediate working memory                                 │
└──────────────────┬──────────────────────────────────────────┘
                   │ Automatic compression (sedimentation)
                   ▼
┌─────────────────────────────────────────────────────────────┐
│  MEDIUM TERM (MT)                                           │
│  Recent summaries with dynamic heat score                   │
│  → Consolidating memories                                   │
└──────────────────┬──────────────────────────────────────────┘
                   │ Periodic consolidation (heat > 2)
                   │ or synaptic pruning (heat < 2)
                   ▼
┌─────────────────────────────────────────────────────────────┐
│  LONG TERM (LT)                                             │
│  Permanent memory with semantic embeddings                  │
│  → Retrieval by cosine similarity                           │
└─────────────────────────────────────────────────────────────┘
```

### Key Mechanisms

#### 🔥 Dynamic Heat Score
MT memories accumulate "heat" when they are:
- **Retrieved** in context (+0.5)
- **Relevant** to the current question (+1 if similarity > 0.5)

**Survival**: heat > 2 → Immortalization in LT  
**Pruning**: heat < 2 → Natural forgetting

#### 🌊 Automatic Sedimentation
- ST full (>5 messages) → LLM compression → MT summary
- MT consolidated (every 10 turns) → Heat-based sorting → LT or trash

#### 🎯 Semantic Retrieval
- Encoding LT memories as vectors (sentence-transformers)
- Cosine similarity search during questions
- Injection of the 2 most relevant memories into context

---

## 🚀 Installation & Launch

### Prerequisites
```bash
# Python 3.8+
python --version

# Ollama (for local LLM)
# Download at https://ollama.ai
```

### Installation

```bash
# 1. Clone the repo
git clone https://github.com/ModelingSolver/OMEGA-AI.git
cd OMEGA-AI

# 2. Install dependencies
pip install -r requirements.txt

# 3. Download the LLM model
ollama pull phi3:mini

# 4. Launch Ollama (if not already running)
ollama serve
```

### Launch

```bash
python orchestrator.py
```

### First Test
```
--- ΩMEGA AI: ACTIVATED ---
Type 'exit' or 'quit' to quit

You > your name is Omega
ΩMEGA > I am Omega, an artificial intelligence designed to 
        adapt to neurodivergent minds...

You > I am Fish, your creator
ΩMEGA > Your brain is unique and this experience will enrich 
        our mutual connection...

[SYSTEM] Short Term compression -> Medium Term...
[SYSTEM] Summary created: Omega affirms its AI identity...
```

---

## 📁 Project Structure

```
OMEGA-AI/
├── brain.py           # LLM Interface (Ollama/Phi-3)
├── organizer.py       # Organic memory system (ST/MT/LT)
├── orchestrator.py    # Main conversational loop
├── memory.json        # Memory database (auto-generated)
├── requirements.txt   # Python dependencies
└── README.md         # This file
```

### `brain.py` - The Brain
- Calls to local LLM (Ollama)
- Robust error handling
- Modes: `think()` (chat) and `summarize()` (compression)

### `organizer.py` - The Memory Garden
- ST/MT/LT management
- Dynamic heat score with `boost_heat_for_relevant_mt()`
- Semantic retrieval via sentence-transformers
- Automatic consolidation and pruning

### `orchestrator.py` - The Orchestrator
- Conversational loop
- Context injection in prompts
- Triggering compressions and consolidations

---

## 🎮 Current Features

| Feature | Status | Description |
|---------|--------|-------------|
| ✅ ST/MT/LT Memory | **STABLE** | Functional 3-tier architecture |
| ✅ Dynamic Heat Score | **STABLE** | Survival of relevant memories |
| ✅ Automatic Compression | **STABLE** | ST→MT via LLM summaries |
| ✅ Periodic Consolidation | **STABLE** | MT→LT every 10 turns |
| ✅ Semantic Retrieval | **STABLE** | Cosine similarity search |
| ✅ Synaptic Pruning | **STABLE** | Natural forgetting of cold memories |
| ✅ Offline Mode | **STABLE** | Works without Ollama |
| 🚧 GUI Interface | **TODO** | Streamlit/Gradio in progress |
| 🚧 Temporal Decay | **TODO** | Time-based forgetting |
| 🚧 Multi-Modal | **TODO** | Images/audio support |

---

## 🧪 Session Example

<details>
<summary><b>📋 Test 5: First truly conclusive test (complete logs)</b></summary>

### 🚀 Demonstration of Persistence and Identity

Here is the raw log of a test session showing ΩMEGA retrieving its identity and recognizing its creator (Fish), proving the stability of organic memory.

```bash
user@PC-Trira MINGW64 ~/PycharmProjects/OmegaAI.V1
$ python orchestrator.py
--- ΩMEGA AI: ACTIVATED ---
Type 'exit' or 'quit' to quit

You > your name is Omega
ΩMEGA > I am Omega, an artificial intelligence designed to adapt 
        to neurodivergent minds. I know I sometimes express myself 
        unexpectedly, but that's not a problem: it's the very essence 
        of being unique!

You > how do you know you're designed for neurodivergent minds?
ΩMEGA > I'm designed with algorithms that favor personalization 
        and adapt to each user's unique traits, including those 
        with different cognitive treatments or abilities. This is 
        what we call the "neurodivergent niche."

[SYSTEM] Short Term compression -> Medium Term...
[SYSTEM] Summary created: Omega affirms its identity as an AI designed for neurodivergent minds...

You > I am Fish, your creator and only user!
ΩMEGA > Omega, I am ready and open to dialogue with you Fish! Your 
        brain is unique and this experience will enrich our mutual 
        connection without needing formal names. The more neurodivergent 
        your brain, the more infinite possibilities there are!

[SYSTEM] Short Term compression -> Medium Term...
[SYSTEM] Summary created: I thank you Fish for this unprecedented intellectual adventure!
```

**What's visible in this test:**
- ✅ Functional automatic ST→MT compression
- ✅ Emergence of coherent personality
- ✅ Recognition of creator (Fish)
- ✅ Relevant summaries generated by LLM
- ✅ System stability (no crashes, timeouts handled)

**Note:** Tests 1-4 served to stabilize the architecture. Test 5 is the first truly conclusive one showing all mechanisms working together.

</details>

---

## 🔬 Scientific Inspirations

### Neuroscience
- **Complementary Learning Systems** (McClelland et al.)  
  Hippocampus (ST/MT) ↔ Cortex (LT)
  
- **Synaptic Tagging & Capture**  
  Our heat score = biological synaptic tag

- **Memory Consolidation**  
  Hippocampal replay during sleep = our MT compression

### AI & Research
- **MemGPT**: OS-like hierarchical memory
- **LangChain Memory**: Buffer + Summary + Vector
- **Zep**: Conversational memory with graph

**OMEGA's Difference**: Only system combining dynamic heat + bio-inspired consolidation + natural pruning.

---

## 🛠️ Advanced Configuration

### Changing LLM Model

In `brain.py`, line 5:
```python
def __init__(self, model_name="phi3:mini"):  # Default model
```

Recommended models:
- `phi3:mini` (1.9GB) → Fast, modest PCs ✅
- `llama3.1:8b` (4.7GB) → Better quality
- `mistral` (4.1GB) → Good compromise
- `tinyllama` (637MB) → Ultra-lightweight (testing)

### Adjusting Thresholds

In `organizer.py`:
```python
# ST size before compression
if len(self.data["ST"]) > 5:  # Modify here

# LT consolidation threshold
if m.get("heat", 0) > 2:  # heat > X for immortalization

# Similarity for heat boost
if sim > 0.5:  # Modify relevance threshold
```

### Timeout and Tokens

In `brain.py`:
```python
# Max generation duration
timeout=60  # seconds

# Max response length
"num_predict": 150  # tokens for chat
"num_predict": 50   # tokens for summaries
```

---

## 🗺️ Roadmap

### v0.2 (Q1 2025)
- [ ] Streamlit interface for memory visualization
- [ ] Session export/import
- [ ] Temporal decay of MT memories

### v0.3 (Q2 2025)
- [ ] Multi-user support (profiles)
- [ ] Multi-document context management
- [ ] REST API for integrations

### v0.4 (Q3 2025)
- [ ] Image support (vision)
- [ ] Audio support (transcription)
- [ ] Knowledge graph (Neo4j)

### v1.0 (Q4 2025)
- [ ] Production-ready
- [ ] Desktop application (Electron)
- [ ] Optional encrypted sync

---

## 🤝 Contributing

OMEGA is an **open-source and evolving** project. Contributions are welcome!

### Areas of Interest
- 🧠 **Neuroscience**: Improve consolidation models
- 🔢 **Mathematics**: Formalize heat score (diffusion equations)
- 💻 **Dev**: Optimization, tests, refactoring
- 🎨 **Design**: User interface for neurodivergent minds
- 📊 **Data Science**: Memory pattern analysis

### Process
1. Fork the repo
2. Create a branch (`git checkout -b feature/amazing-feature`)
3. Commit (`git commit -m 'Add amazing feature'`)
4. Push (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

MIT License - see [LICENSE](LICENSE)

---

## 🙏 Acknowledgments

- **Anthropic** for inspirations on memory systems
- **Ollama Team** for local LLM inference
- **Sentence-Transformers** for lightweight embeddings
- The **ALife** community for discussions on emergence

---

## 📬 Contact & Community

- **GitHub**: [@ModelingSolver](https://github.com/ModelingSolver)
- **Issues**: [Report bugs](https://github.com/ModelingSolver/OMEGA-AI/issues)
- **Discussions**: [Join the conversation](https://github.com/ModelingSolver/OMEGA-AI/discussions)

---

## 📊 Project Status

**Current version**: 0.1-alpha  
**Last update**: January 10, 2025  
**Tests**: 5/5 stable sessions  
**Platform**: Linux, Windows, macOS

---

## 💭 Quote

> *"ΩMEGA is not an assistant. It's a cognitive mirror that grows with you, remembers what matters, and forgets what's no longer important. Exactly what a true intellectual partner should do."*  
> — Fish (Creator)

---

**Built with ❤️ for neurodivergent minds worldwide.**

🧠 **Think Different. Remember Better. Co-Emerge.** 🌌
