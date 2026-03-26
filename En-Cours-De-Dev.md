📅 10 Janvier 2026 : Diagnostic de saturation 
 Lien : https://youtu.be/JtOW6oLL2MU

    "Ça marche mais c’est super lent... ok super... on dirait un bug... peut-être une des couches de mémoire qui sature. Je pense que tout le délire ça va être ça... Wai c’est ça, il y avait la couche qui saturait. Faudrait qu’il embedde de MT à LT aussi... mais tout est lent, tout est lent... WOOO c’est pas bon comme résumé ça ! Okay ! Faut changer tout, faut changer tout... (sifflement). Je chante, quand ça marche pas c'est là où t'apprends hein ! Ben c’est ce qu’il faut se dire hein... Dans mon pov terminal... Wai j’ai pas fait d’interface un peu jolie, ou même d’interface tout court encore. Ok j’ai compris c’est une saturation des couches mémoires. Ok on va régler ça !"

Le constat : Pas de chichi, pas d'interface. Juste le moteur qui s'étouffe sur un laptop de base. C'est le moment où je capte que le goulot d'étranglement, c'est la gestion des couches CT/MT/LT. C'est lent, c'est moche, mais le diagnostic est posé.




🪵 26/03/2026 DEV LOG #01 : ΩMEGA — Efficience Mémorielle et Souveraineté Locale

Objectif : Validation d'une architecture à consommation mémoire constante pour LLM local (Mistral 7B) sur matériel grand public (Intel i7).
📊 Analyse de Performance (Stress Test : 200 tours)

https://www.youtube.com/watch?v=Pev7Z3lxKQg

    Gestion de la RAM : Homéostasie confirmée. Le système a maintenu une empreinte stable entre 130 Mo et 400 Mo tout au long de la session. Contrairement aux approches RAG classiques ou LangChain, le processus de "Sédimentation" (CT → MT → LT) permet de briser la croissance linéaire du contexte, évitant ainsi la saturation RAM.

    Charge CPU et Thermique : Le cycle de "respiration" mémorielle permet de lisser la charge. L'alternance entre l'inférence active et la compression en arrière-plan prévient le thermal throttling (bridage thermique) et assure la viabilité du système sur le long terme sans GPU dédié.

    Stockage Stratifié : Validation du transfert automatique des données entre trois niveaux de volatilité, garantissant que seules les informations à haute valeur ajoutée atteignent le stockage persistant.

⚠️ Dette Technique et Points de Rupture Identifiés

    Dédoublonnage Sémantique : La mémoire à long terme (LT) manque actuellement d'un filtre de similarité. En cycle de haute fréquence, cela génère des redondances ("effet d'écho") qui polluent la base de connaissances.

    Divergence du Recall : Échec du test de rappel suite à un conflit de chemin d'accès (désynchronisation entre l'environnement de test et la base de données de production).

    Latence I/O : Des pics à 60s ont été observés lors des phases critiques de compression simultanée à l'inférence.

Statut : Architecture validée. Optimisation logique en cours.
Philosophie : Local-first. Privacy by design. Sobriété numérique. 🛡️
