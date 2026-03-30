# 🏋️‍♂️ ΩMEGA - BenchPress Logs

> "Pushing the boundaries of local inference on legacy hardware."
>
> Statut : Semi-échec / Semi-réussite (DB wipe accidentel) 😅

Vidéo du run : Omega Benchpress - [YouTube](https://www.youtube.com/watch?v=Pev7Z3lxKQg)

Note : Les échecs de rappel (Recall) sont dus à une purge complète de la base de données de test juste avant le run.

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
- **Final RAM (Round 200):** 130 MB (Sedimentation active)
- **CPU Temp:** Stable (Breathing cycles functional)

### 🎯 Functional Results
- **ST Memory (Short-Term):** 100% Fluid.
- **MT Consolidation (Medium-Term):** 100% Accurate summarization.
- **LT Recall (Long-Term):** 100% but **RECALL FAILED** (Path sync error in `test_organique.json`).
- **Semantic Drift:** Observed at Round 180 (needs de-duplication).

### 📝 Raw Thoughts
"Le système respire enfin. La courbe de RAM n'est plus une rampe vers le crash, c'est un plateau. 
 Le KO contre le RAG classique est validé techniquement, reste à fixer la précision du Recall."


 <img width="1013" height="548" alt="Capture d&#39;écran 2026-03-26 070524" src="https://github.com/user-attachments/assets/eb576f16-5e27-439d-997b-df3792ba5b11" />


<img width="1064" height="338" alt="Capture d&#39;écran 2026-03-26 070535" src="https://github.com/user-attachments/assets/a9090002-c986-4f5d-aa1a-0c8924744997" />


<img width="1054" height="251" alt="Capture d&#39;écran 2026-03-26 070547" src="https://github.com/user-attachments/assets/b011d510-9a8b-4339-9b3e-b44d654ea6ca" />


 ## 🧪 Session BP-02 (2026-03-30) - Sprint "Stabilité & Sédimentation"


Contexte : Correction de la fuite de données CT → MT et analyse de la précision sémantique.

### 📈 Métriques de Performance


    Recall Rate : 33.3% (Passage de 0% à 33.3% — Progression technique confirmée)

    Initial RAM: 357.73 MB

    Peak RAM (Round 18): 404.31 MB

    Final RAM (Round 239): 134.65 MB (Sedimentation active)

    CPU Temp: Stable (Moyenne 6.97% | Max 56.9% — Cycles de respiration fonctionnels)


    Memory Slots : Croissance linéaire. La tuyauterie CT -> MT est désormais étanche.


### 🎯 Analyse Technique (Post-Mortem)


    Victoire : La sédimentation par message individuel fonctionne. Le système ne "perd" plus d'informations lors de l'archivage.


    Identification du "Recall Gap" : 1. Data d'entrée : Erreur de formatage sur les données sources, créant un décalage lors de la récupération.

    2. Embedding Agressif : Le modèle d'embedding actuel sature trop vite, ce qui occasionne des pertes sémantiques.


    LTD (Long Term Depression) : Probleme de seuils de mécanisme d'oubli actif, causant un élagage insufisant.


### 🛠️ Roadmap Sprint BP-03


    Normalisation Data : Nettoyage des entrées pour garantir l'alignement sémantique.


    Fine-tuning de l'Embedding : Ajustement des seuils de similarité pour réduire l'agressivité du modèle et regagner de la granularité.


    Filtre Anti-Doublons LT : Implémentation d'un check avant immortalisation pour éviter la redondance.


    "Le saut à 33% valide l'architecture. Le reste est une question de réglage de précision sur l'embedding et de qualité de data."

