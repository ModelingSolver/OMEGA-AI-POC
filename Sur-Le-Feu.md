🔥 Sur Le Feu : Roadmap & Travaux en Cours

Ce document trace l'évolution immédiate d'ΩMEGA AI, de l'état de prototype fonctionnel à celui d'exocortex cognitif de grade recherche.
1. Migration Linux & Montée en Puissance 🐧

Actuellement, Windows consomme environ 8 Go de RAM, ce qui bride le déploiement de modèles plus lourds.

    Action : Migration vers un environnement Linux dédié (Dual Boot).

    Objectif : Libérer les ressources pour remplacer Phi-3 par Mistral-Nemo (12B) ou Llama 3.1 (8B).

    Impact : Une capacité de raisonnement accrue pour le "Greffier" (résumés) et une meilleure saisie des nuances du français et de l'argot pour l'utilisateur.

2. Affinement du "Heat Score" (LTP/LTD) 🧠

Le mécanisme est fonctionnel mais nécessite un réglage empirique précis.

    Action : Test du seuil de similarité à 0.35 sur des sessions réelles de longue durée.

    Action : Implémentation du Temporal Decay (Érosion Temporelle). Comme la mémoire biologique, un souvenir "chaud" non consulté pendant 48h doit perdre naturellement en température.

    Action : Formalisation du seuil d'"Immortalisation" (Heat > 2).

3. Recherche Empirique & Retours Humains 🔬

Passer du code à l'humain.

    Action : Tests internes avec des "cobayes" (bêta-testeurs) issus de la communauté neuro-atypique (TDAH, TSA, HPI).

    Collecte de données : Observer comment ΩMEGA gère les "trous de fonctions exécutives" (ex: se souvenir d'une tâche citée il y a 3h ou d'un changement d'humeur).

    Pont Académique : Prise de contact avec les chercheurs en neuropsycho (LPNC/GIN Grenoble) pour valider l'impact de l'architecture sur la charge cognitive.

4. Visualisation & Interface (L'effet Miroir) 🖥️

Le terminal, c'est bien, mais un "Miroir Cognitif" a besoin d'un visage.

    Action : Développement d'une interface Streamlit/Gradio.

    Fonctionnalité : Une "Heatmap de la mémoire" permettant à l'utilisateur de voir quels souvenirs sont "brûlants" (MT) et lesquels "coulent" vers l'archive profonde (LT).

5. Objectifs Bourse NLNet 🎯

Cette roadmap s'aligne sur nos engagements :

    Souveraineté Numérique : 100% local, aucune télémétrie.

    Impact Social : Focus spécifique sur l'accessibilité cognitive et la neuro-inclusion.

    Science Ouverte : Documentation du processus de co-émergence entre esprits atypiques et mémoire stratifiée d'IA.


25/02/2026
    ΩMEGA AI — Roadmap Sprint 1 Mois
Objectif : Passer de POC fonctionnel à projet scientifiquement crédible

Semaine 1 — Stabilité & Performance

Optimiser la gestion mémoire pour fonctionner correctement sur petit matériel
Implémenter le Temporal Decay (dégradation temporelle du heat score)
Logging propre : chaque opération mémoire tracée et mesurable

Semaine 2 — Benchmarks & Métriques

Définir les métriques clés :

Latence de rappel (ST / MT / LT)
Pertinence des souvenirs injectés en contexte (score cosine moyen)
Consommation RAM selon le modèle LLM utilisé
Taux de pruning vs taux de consolidation sur session longue


Benchmark comparatif vs MemGPT sur scénarios identiques
Documenter les résultats bruts dans /benchmarks/

Semaine 3 — GUI Minimale & User Research

Interface Streamlit ou Gradio minimaliste :

Fenêtre conversation
Visualisation Memory Heatmap (ST/MT/LT en temps réel)
Indicateur de heat score visible


Finaliser les entretiens user research (objectif : 8-10 participants)
Synthèse des patterns HPI / TSA / TDAH

Semaine 4 — Documentation & Outreach

README mis à jour avec benchmarks et résultats
Rédaction synthèse user research publiable (anonymisée)
Dossier NLNet finalisé
Relance LPNC/GIN Grenoble avec résultats concrets en main
Préparer le pitch : ΩMEGA vs MemGPT en 5 slides


Livrable Final (J+30)

ΩMEGA stable sur Mistral/Llama 3.1 sur PC modeste
Benchmark documenté vs MemGPT
GUI minimale fonctionnelle
User research complète (10 participants)
Dossier prêt pour collaboration académique


"On revient dans un mois quand on aura mis sa race à MemGPT."
— Fish, Architecte Organique



NB — Mars 2026
Nous touchons les limites de nos moyens. Matériel en fin de vie, ressources au minimum.
Ce projet engage désormais bien plus que moi — des gens y croient, des gens comptent dessus.
On lâche rien.
Force et résilience. 💪❤️

26/03/2026

🛠 Roadmap v2.1 (Correctifs Immédiats)

    Dédoublonnage par Cosine Similarity : Intégration d'un seuil de similarité avant l'insertion en LT pour garantir une base de données "High Signal".

    Unification des Flux DB : Migration vers un flux JSON/SQLite unique pour empêcher toute divergence d'état entre les tests et l'usage réel.

    Optimisation du Greffier : Raffinement des prompts de résumé pour réduire le nombre de tokens générés et abaisser la latence.

