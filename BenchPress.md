# 🏋️‍♂️ ΩMEGA - BenchPress Logs

> "Pushing the boundaries of local inference on legacy hardware."
>
> Status: Semi-failure / Semi-success (Accidental DB wipe) 😅

Run Video: Omega Benchpress - [YouTube](https://www.youtube.com/watch?v=g5IwhkT3ruk)

Note: The Recall failures are due to a complete purge of the test database performed just before the run.

## 📊 Summary of Records
- **Max Conversations Rounds:** 200 (Confirmed 26/03/2026)
- **RAM Floor:** 130 MB
- **RAM Ceiling:** 400 MB
- **Engine:** Mistral 7B (via Ollama)
- **Host:** Intel i7 (Mobile) - "The Dying Laptop"

---

## 🧪 Session BP-01 (2026-03-26)
**Context:** Stress-test initial post-migration.

### 📈 Resource Metrics
- **Initial RAM:** 130 MB
- **Peak RAM (Round 5/8):** 403 MB
- **Final RAM (Round 200):** 134 MB  (Sedimentation active)
- **CPU Temp:** Stable (Breathing cycles functional)

### 🎯 Functional Results
- **ST Memory (Short-Term):** 100% Fluid.
- **MT Consolidation (Medium-Term):** 100% Accurate summarization.
- **LT Recall (Long-Term):** 100% but **RECALL FAILED** (Path sync error in `test_organique.json`).
- **Semantic Drift:** Observed at Round 180 (needs de-duplication).

### 📝 Raw Thoughts
"Le système respire enfin. La courbe de RAM n'est plus une rampe vers le crash, c'est un plateau. 
 Le KO contre le RAG classique est validé techniquement, reste à fixer la précision du Recall."

 <img width="1013" height="548" alt="Capture d&#39;écran 2026-03-26 070524" src="https://github.com/user-attachments/assets/d2a09351-2b70-4e9b-90d9-22c2ae92f5bf" />

<img width="1064" height="338" alt="Capture d&#39;écran 2026-03-26 070535" src="https://github.com/user-attachments/assets/a7d434ca-33cf-4bdf-8aa6-44a4c44e824a" />

<img width="1054" height="251" alt="Capture d&#39;écran 2026-03-26 070547" src="https://github.com/user-attachments/assets/210a629e-6c93-44a6-96f2-92ac2410e644" />




🧪 Session BP-02 (2026-03-30) - Sprint "Stability & Sedimentation"

<https://www.youtube.com/watch?v=yhKsKL64AIk>
       

Context: Fixed the CT → MT data leakage and analyzed semantic precision.
📈 Performance Metrics

    Recall Rate: 33.3% (Up from 0% to 33.3% — Technical progression confirmed)

    Initial RAM: 357.73 MB

    Peak RAM (Round 18): 404.31 MB

    Final RAM (Round 239): 134.65 MB (Active Sedimentation)

    CPU Temp: Stable (Average 6.97% | Max 56.9% — "Breathing cycles" fully functional)

    Memory Slots: Linear growth. The CT -> MT pipeline is now fully airtight.

🎯 Technical Analysis (Post-Mortem)

    Success: Individual message sedimentation is operational. The system no longer "drops" information during archiving.

    Recall Gap Identification: 1. Input Data: Formatting errors in source data, creating a mismatch during retrieval.
    2. Aggressive Embedding: The current embedding model saturates too quickly, causing semantic loss.

    LTD (Long Term Depression): Issues with active forgetting mechanism thresholds, resulting in insufficient pruning.

🛠️ Roadmap Sprint BP-03

    Data Normalization: Cleaning inputs to ensure perfect semantic alignment.

    Embedding Fine-tuning: Adjusting similarity thresholds to reduce model "aggressiveness" and regain granularity.

    LT Anti-Duplication Filter: Implementing a pre-immortalization check to prevent redundancy.

    "The jump to 33.3% validates the architecture. The rest is a matter of fine-tuning embedding precision and data quality."

    RAM floor       RAM peak                          Avg. latency        Recall
    131 MB          404 MB                            33.8s               PARTIAL
   après T100+      T5–T20 (chargement modèle)        i7 mobile, local    S_RECALL 1/3 · S_PRECISION 1/3
 
<img width="981" height="300" alt="image" src="https://github.com/user-attachments/assets/9cd89062-4ab1-4ad7-a5c0-f6041f99d94e" />

<img width="981" height="272" alt="image" src="https://github.com/user-attachments/assets/75bd961f-d8fc-48cd-ac6e-8cf19c29837e" />
