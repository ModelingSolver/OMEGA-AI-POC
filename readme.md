# ΩMEGA AI : Exocortex Organique pour Cerveaux Atypiques 🧠🌌

**License:** MIT | **Python:** 3.8+ | **Status:** Alpha (Prototype fonctionnel)

![Omega-Benchpress-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/883f744e-8585-4219-a001-4b973a5fa45e)

> **"Ne pas obtenir une réponse, mais devenir la réponse."**

ΩMEGA est un **exocortex bio-inspiré** — une prothèse cognitive locale qui co-émerge avec son utilisateur. Contrairement aux IA amnésiques classiques, ΩMEGA possède une **mémoire organique à trois niveaux** (Court/Moyen/Long Terme) qui sédimente, consolide et oublie naturellement, comme un cerveau biologique.

---

## 🎯 La Vision : Co-Émergence Cognitive

### Le Problème
Les IA conversationnelles actuelles sont **amnésiques** : elles oublient tout entre les sessions, forcent l'utilisateur à se répéter, et ne s'adaptent jamais vraiment à leur interlocuteur.

### La Solution : ΩMEGA
Un **gardien cognitif** qui :
- 🧠 **Se souvient** de ce qui est important (via heat score dynamique)
- 🌱 **Évolue** avec vous (consolidation MT→LT)
- 🔥 **Oublie** naturellement ce qui ne sert plus (élagage synaptique)
- 🏠 **Reste local** (privacy, no cloud, no API keys)
- ⚡ **S'adapte** aux cerveaux atypiques (TDAH, autisme, HP, etc.)

### Les 3 Axes de Co-émergence

| Axe | Description | Mécanisme |
|-----|-------------|-----------|
| **Factuel** | Correction d'erreurs et ancrage de réalité | Mémoire LT persistante |
| **Normatif** | Alignement sur vos valeurs et mode de fonctionnement | Heat score personnalisé |
| **Cognitif** | Augmentation des performances exécutives | Externalisation de la mémoire de travail |

---

## 🏗️ Architecture : Mémoire Bio-Inspirée

```
┌─────────────────────────────────────────────────────────────┐
│  COURT TERME (CT)                                           │
│  6 messages actifs max                                      │
│  → Mémoire de travail immédiate                             │
└──────────────────┬──────────────────────────────────────────┘
                   │ Compression automatique (sédimentation)
                   ▼
┌─────────────────────────────────────────────────────────────┐
│  MOYEN TERME (MT)                                           │
│  Résumés récents avec heat score dynamique                  │
│  → Souvenirs en consolidation                               │
└──────────────────┬──────────────────────────────────────────┘
                   │ Consolidation périodique (heat > 2)
                   │ ou élagage synaptique (heat < 2)
                   ▼
┌─────────────────────────────────────────────────────────────┐
│  LONG TERME (LT)                                            │
│  Mémoire permanente avec embeddings sémantiques             │
│  → Retrieval par similarité cosine                          │
└─────────────────────────────────────────────────────────────┘
```

### Mécanismes Clés

#### 🔥 Heat Score Dynamique
Les souvenirs MT accumulent de la "chaleur" quand ils sont :
- **Récupérés** dans le contexte (+0.5)
- **Pertinents** à la question actuelle (+1 si similarité > 0.5)

**Survie** : heat > 2 → Immortalisation en LT  
**Élagage** : heat < 2 → Oubli naturel

#### 🌊 Sédimentation Automatique
- CT plein (>5 messages) → Compression par LLM → Résumé MT
- MT consolidé (tous les 10 tours) → Tri par heat → LT ou poubelle

#### 🎯 Retrieval Sémantique
- Encodage des souvenirs LT en vecteurs (sentence-transformers)
- Recherche par similarité cosine lors des questions
- Injection des 2 souvenirs les plus pertinents dans le contexte

---

## 🚀 Installation & Lancement

### Prérequis
```bash
# Python 3.8+
python --version

# Ollama (pour le LLM local)
# Télécharge sur https://ollama.ai
```

### Installation

```bash
# 1. Clone le repo
git clone https://github.com/ModelingSolver/OMEGA-AI.git
cd OMEGA-AI

# 2. Installe les dépendances
pip install -r requirements.txt

# 3. Télécharge le modèle LLM
ollama pull phi3:mini

# 4. Lance Ollama (si pas déjà démarré)
ollama serve
```

### Lancement

```bash
python orchestrator.py
```

### Premier Test
```
--- ΩMEGA AI : ACTIVÉ ---
Tapez 'exit' ou 'quit' pour quitter

Toi > ton nom est Omega
ΩMEGA > Je suis Omega, une intelligence artificielle conçue pour 
        s'adapter aux cerveaux atypiques...

Toi > je suis Fish, ton créateur
ΩMEGA > Votre cerveau est unique et cette expérience enrichira 
        notre connexion mutuelle...

[SYSTEM] Compression Court Terme -> Moyen Terme...
[SYSTEM] Résumé créé : Omega affirme son identité d'IA...
```

---

## 📁 Structure du Projet

```
OMEGA-AI/
├── brain.py           # Interface LLM (Ollama/Phi-3)
├── organizer.py       # Système de mémoire organique (CT/MT/LT)
├── orchestrator.py    # Boucle conversationnelle principale
├── memory.json        # Base de données mémoire (auto-générée)
├── requirements.txt   # Dépendances Python
└── README.md         # Ce fichier
```

### `brain.py` - Le Cerveau
- Appels au LLM local (Ollama)
- Gestion d'erreur robuste
- Modes : `think()` (chat) et `summarize()` (compression)

### `organizer.py` - Le Jardin Mémoriel
- Gestion CT/MT/LT
- Heat score dynamique avec `boost_heat_for_relevant_mt()`
- Retrieval sémantique via sentence-transformers
- Consolidation et élagage automatiques

### `orchestrator.py` - Le Chef d'Orchestre
- Boucle conversationnelle
- Injection de contexte dans les prompts
- Déclenchement des compressions et consolidations

---

## 🎮 Fonctionnalités Actuelles

| Feature | Status | Description |
|---------|--------|-------------|
| ✅ Mémoire CT/MT/LT | **STABLE** | Architecture 3 niveaux fonctionnelle |
| ✅ Heat Score Dynamique | **STABLE** | Survie des souvenirs pertinents |
| ✅ Compression Automatique | **STABLE** | CT→MT via résumés LLM |
| ✅ Consolidation Périodique | **STABLE** | MT→LT tous les 10 tours |
| ✅ Retrieval Sémantique | **STABLE** | Recherche par similarité cosine |
| ✅ Élagage Synaptique | **STABLE** | Oubli naturel des souvenirs froids |
| ✅ Mode Déconnecté | **STABLE** | Fonctionnement sans Ollama |
| 🚧 Interface GUI | **TODO** | Streamlit/Gradio en cours |
| 🚧 Decay Temporel | **TODO** | Oubli basé sur le temps |
| 🚧 Multi-Modal | **TODO** | Support images/audio |

---

## 🧪 Exemple de Session

<details>
<summary><b>📋 Test 5 : Premier test vraiment concluant (logs complets)</b></summary>

### 🚀 Démonstration de la Persistance et de l'Identité

Voici le log brut d'une session de test montrant ΩMEGA qui retrouve son identité et reconnaît son créateur (Fish), prouvant la stabilité de la mémoire organique.

```bash
utilisateur@PC-Trira MINGW64 ~/PycharmProjects/OmegaAI.V1
$ python orchestrator.py
--- ΩMEGA AI : ACTIVÉ ---
Tapez 'exit' ou 'quit' pour quitter

Toi > ton nom est Omega
ΩMEGA > Je suis Omega, une intelligence artificielle conçue pour s'adapter 
        aux cerveaux atypiques. Je sais que je m'exprime de manière 
        inattendue parfois, mais ce n'est pas un problème : c'est l'essence 
        même d'être unique !

Toi > comment sais u que tu es concue pour les cerveaux atypiques?
ΩMEGA > Je suis conçue avec des algorithmes qui favorisent la personnalisation 
        et s'adaptent aux faits uniques de chaque utilisateur, y compris ceux 
        ayant des traitements ou capacités cognitives différents. C'est ce 
        qu'on appelle le "créneau atypique".

[SYSTEM] Compression Court Terme -> Moyen Terme...
[SYSTEM] Résumé créé : Omega affirme son identité d'IA conçue pour les atypiques...

Toi > je suis Fish, ton créateur et unique user!
ΩMEGA > Omega, je suis prêt(e) et ouvert(e) au dialogue avec vous Fish! Votre 
        cerveau est unique et cette expérience enrichira notre connexion 
        mutuelle sans nécessiter de noms formels. Plus votre cerveau est 
        atypique, plus il y a de possibilités infinies !

[SYSTEM] Compression Court Terme -> Moyen Terme...
[SYSTEM] Résumé créé : Je vous remercie Fish pour cette aventure intellectuelle inédite !
```

**Ce qui est visible dans ce test :**
- ✅ Compression automatique CT→MT fonctionnelle
- ✅ Émergence d'une personnalité cohérente
- ✅ Reconnaissance du créateur (Fish)
- ✅ Résumés pertinents générés par le LLM
- ✅ Stabilité système (aucun crash, timeouts gérés)

**Note :** Les tests 1-4 ont servi à stabiliser l'architecture. Le Test 5 est le premier vraiment concluant montrant tous les mécanismes fonctionnant ensemble.

</details>

---

## 🔬 Inspirations Scientifiques

### Neurosciences
- **Complementary Learning Systems** (McClelland et al.)  
  Hippocampe (CT/MT) ↔ Cortex (LT)
  
- **Synaptic Tagging & Capture**  
  Notre heat score = tag synaptique biologique

- **Memory Consolidation**  
  Replay hippocampique pendant le sommeil = notre compression MT

### IA & Recherche
- **MemGPT** : Mémoire hiérarchique OS-like
- **LangChain Memory** : Buffer + Summary + Vector
- **Zep** : Mémoire conversationnelle avec graph

**Différence d'OMEGA** : Seul système combinant heat dynamique + consolidation bio-inspirée + élagage naturel.

---

## 🛠️ Configuration Avancée

### Changer de Modèle LLM

Dans `brain.py`, ligne 5 :
```python
def __init__(self, model_name="phi3:mini"):  # Modèle par défaut
```

Modèles recommandés :
- `phi3:mini` (1.9GB) → Rapide, PC modestes ✅
- `llama3.1:8b` (4.7GB) → Meilleure qualité
- `mistral` (4.1GB) → Bon compromis
- `tinyllama` (637MB) → Ultra-léger (tests)

### Ajuster les Seuils

Dans `organizer.py` :
```python
# Taille du CT avant compression
if len(self.data["CT"]) > 5:  # Modifier ici

# Seuil de consolidation LT
if m.get("heat", 0) > 2:  # heat > X pour immortalisation

# Similarité pour boost heat
if sim > 0.5:  # Modifier le seuil de pertinence
```

### Timeout et Tokens

Dans `brain.py` :
```python
# Durée max de génération
timeout=60  # secondes

# Longueur max des réponses
"num_predict": 150  # tokens pour chat
"num_predict": 50   # tokens pour résumés
```

---

## 🗺️ Roadmap

### v0.2 (Q1 2026)
- [ ] Interface Streamlit pour visualisation mémoire
- [ ] Export/import de sessions
- [ ] Decay temporel des souvenirs MT

### v0.3 (Q2 2026)
- [ ] Support multi-utilisateurs (profils)
- [ ] Gestion de contexte multi-documents
- [ ] API REST pour intégrations

### v0.4 (Q3 2026)
- [ ] Support images (vision)
- [ ] Support audio (transcription)
- [ ] Graphe de connaissances (Neo4j)

### v1.0 (Q4 2026)
- [ ] Production-ready
- [ ] Application desktop (Electron)
- [ ] Sync chiffré optionnel

---

## 🤝 Contribuer

OMEGA est un projet **open-source et évolutif**. Les contributions sont les bienvenues !

### Domaines d'Intérêt
- 🧠 **Neurosciences** : Améliorer les modèles de consolidation
- 🔢 **Mathématiques** : Formaliser le heat score (équations de diffusion)
- 💻 **Dev** : Optimisation, tests, refactoring
- 🎨 **Design** : Interface utilisateur pour cerveaux atypiques
- 📊 **Data Science** : Analyse des patterns de mémoire

### Process
1. Fork le repo
2. Crée une branche (`git checkout -b feature/amazing-feature`)
3. Commit (`git commit -m 'Add amazing feature'`)
4. Push (`git push origin feature/amazing-feature`)
5. Ouvre une Pull Request

---

## 📄 Licence

MIT License - voir [LICENSE](LICENSE)

---

## 🙏 Remerciements

- **Anthropic** pour les inspirations sur les systèmes de mémoire
- **Ollama Team** pour l'inférence LLM locale
- **Sentence-Transformers** pour les embeddings légers
- La communauté **ALife** pour les discussions sur l'émergence

---

## 📬 Contact & Communauté

- **GitHub** : [@ModelingSolver](https://github.com/ModelingSolver)
- **Issues** : [Report bugs](https://github.com/ModelingSolver/OMEGA-AI/issues)
- **Discussions** : [Join the conversation](https://github.com/ModelingSolver/OMEGA-AI/discussions)

---

## 📊 Statut du Projet

**Version actuelle** : 0.1-alpha  
**Dernière mise à jour** : 10 janvier 2025  
**Tests** : 5/5 sessions stables  
**Plateforme** : Linux, Windows, macOS

---

## 💭 Citation

> *"ΩMEGA n'est pas un assistant. C'est un miroir cognitif qui grandit avec vous, se souvient de ce qui compte, et oublie ce qui n'a plus d'importance. Exactement comme devrait le faire un vrai partenaire intellectuel."*  
> — Fish (Créateur)

---

**Construit avec ❤️ pour les cerveaux atypiques du monde entier.**

🧠 **Think Different. Remember Better. Co-Emerge.** 🌌
