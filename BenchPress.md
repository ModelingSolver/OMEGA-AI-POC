# 🏋️‍♂️ ΩMEGA - BenchPress Logs

> "Pushing the boundaries of local inference on legacy hardware."
>
> Status: Semi-failure / Semi-success (Accidental DB wipe) 😅

Run Video: Omega Benchpress - [YouTube](https://www.youtube.com/watch?v=Pev7Z3lxKQg)

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
