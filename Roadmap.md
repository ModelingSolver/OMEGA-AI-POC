🚀 What Now? / Current Roadmap

This document tracks the immediate evolution of ΩMEGA AI as it moves from a functional prototype to a research-grade cognitive exocortex.
1. The "Linux Migration" & Power Upgrade 🐧

Current Windows overhead (consuming ~8GB RAM) limits the deployment of advanced models.

    Action: Migration to a dedicated Linux environment (Dual Boot).

    Goal: Freeing resources to swap Phi-3 with Mistral-Nemo (12B) or Llama 3.1 (8B).

    Impact: Higher reasoning quality for the "Greffier" (summarization) and better nuance in French/slang for the user.

2. Refining the "Heat Score" (LTP/LTD) 🧠

The current mechanism is functional but requires empirical fine-tuning.

    Action: Testing the 0.35 similarity threshold in real-world long-duration sessions.

    Action: Implementing Temporal Decay. Just like biological memory, a "hot" memory that isn't accessed for 48 hours should lose heat naturally.

    Action: Formalizing the "Immortalization" threshold (Heat > 2).

3. Empirical Research & Human Feedback 🔬

Moving from code to humans.

    Action: Internal testing with "cobayes" (beta-testers) from the neurodivergent community (ADHD, ASD, Giftedness).

    Data Collection: Observing how ΩMEGA handles "executive function gaps" (e.g., remembering a task mentioned 3 hours ago or a mood shift).

    Academic Bridge: Reaching out to neuro-psychology researchers (LPNC/GIN Grenoble) to validate the architecture's impact on cognitive load.

4. Visualization & UI (The "Mirror" Effect) 🖥️

A terminal is good, but a "Cognitive Mirror" needs a face.

    Action: Developing a Streamlit/Gradio interface.

    Feature: A "Memory Heatmap" allowing the user to see which memories are currently "hot" (MT) and which are "sinking" into the deep archive (LT).

5. NLNet Grant Objectives 🎯

This roadmap aligns with our commitment to:

    Digital Sovereignty: 100% local, no telemetry.

    Social Impact: Specific focus on cognitive accessibility and neuro-inclusion.

    Open Science: Documentation of the co-emergence process between atypical minds and stratified AI memory.


25/02/2026 ΩMEGA AI — Sprint 1 Roadmap
Objective: Move from a functional POC to a scientifically credible project

Week 1 — Stability & Performance

Optimize memory management to run properly on low-end hardware

Implement Temporal Decay (time-based decay of the heat score)

Clean logging: every memory operation tracked and measurable

Week 2 — Benchmarks & Metrics

Define key metrics:

Recall latency (ST / MT / LT)

Relevance of injected memories in context (average cosine score)

RAM consumption depending on the LLM model used

Pruning rate vs. consolidation rate over long sessions

Comparative benchmark vs MemGPT under identical scenarios

Document raw results in /benchmarks/

Week 3 — Minimal GUI & User Research

Minimal Streamlit or Gradio interface:

Conversation window

Memory Heatmap visualization (ST/MT/LT in real time)

Visible heat score indicator

Finalize user research interviews (goal: 8–10 participants)

Synthesis of HPI / ASD / ADHD patterns

Week 4 — Documentation & Outreach

Update README with benchmarks and results

Write publishable (anonymized) user research summary

Finalize NLNet application

Follow up with LPNC / GIN Grenoble with concrete results in hand

Prepare the pitch: ΩMEGA vs MemGPT in 5 slides

Final Deliverable (D+30)

ΩMEGA stable on Mistral / Llama 3.1 on a modest PC

Documented benchmark vs MemGPT

Functional minimal GUI

Complete user research (10 participants)

Dossier ready for academic collaboration

“We’ll come back in a month once we’ve completely crushed MemGPT.”
— Fish, Organic Architect




NB — March 2026
We are pushing the limits of what we have. Aging hardware, bare minimum resources. 
This project now carries more than just me — people believe in it, people count on it. 
We don't let go. 
Strength and honor. 💪❤️
