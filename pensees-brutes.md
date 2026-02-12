Omega est un projet de llm local ….

Postulat de la co-émergence.
De par leur archi /structure les llm ont une certaines plasticité et faculté d'adaptation à user; cette adaptation de user au llm et du llm a user permet une co-émergence.
Les modèles qu'ils soient locaux ou online sont " amnésique " ce qui limite la qualité d'interaction et la "co emergence ia/humain".
Le postulat de r&d Omega AI est le suivant:
Une mémoire "efficace" permettrait une meilleure qualité interactionnelle du lm et une meilleure co emergence llm/user..
Ceci sans toucher aux poids du llm, sans passer par un recalibrage interne qui serait efficace mais énergivore et chronophage en local ( et impossible sur un modèle non local! ).

Apres avoir envisagé et testé des boucles de recalibrage externes ( systèmes rags ), cela est apparu évident que le système de mémoire cumulative classique pour "rag" est limité.
Aussi après avoir observé et réfléchi sur la mémoire chez les humains, j'ai eu l'idée d'une mémoire Organic like externe pour llm local.

Le projet voulant considérer trois axes de base que sont 
- axe factuel ou correctifs 
- axe normatif ou éthique
- axe cognitif ou de performance

L'implémentation d'un organe de mémoire organic like permettrait un meilleur alignement factuel et cognitif, avec une possibilité d'adaptation a l'éthique de user.

Ceci ouvre également une perspective se souveraineté de part le stockage et le confinement de la data user en local et une alternative réelle aux grands modelés commerciaux offrant non dépendance aux infrastructures privées et respect de la vie privée.


Je souhaite décliner ce projet en deux partie…
Une première partie consistant en une alternative grand publique locale et souveraine,
et une deuxième partie comme outil d'aide aux cerveaux atypiques ( hpi, tdah, tsa… )
Apres des premiers essais, échecs et un poc fonctionnel le projet consiste en :
- dev d'un llm local avec mémoire organic like 
- Réflexion et dev d'outils thérapeutiques ou llm d'aide aux personnes souffrant d'atypie cérébrale…


Le but ne sera pas de dev une toute puissante AGI ou une super IA mais de dev des outils fonctionnels qui ouvriront un peu plus la voix de la recherche et du développement de modelés et d'outils locaux et humains.. 



1. Memoire pour llm:

Les premiers essais ont consisté a constater l'ineficacité de modeles "rags" classiques avec memoire archive, encyclopedie like...
Les problemes sont divers:
Le cumul et la lourdeur,
le manque d agiité ou de pertinence dans le traitement de la dat ( ecriture et utilisation,.)
des problemes de puissance ( gestion de la memoire archive like plus llm local.. )
puissance de process exponentielle
Ce type de memoire a donc vite montré ses limites..

Aussi me suis je naivement permis une reflexion sur la mémoire "humaine"!
Me concentrant sur ce qu on pouvait constater de son fonctionnement plus que sur la realité biologique j'ai vite isolé un axe de dev:

La mémoire organisée en trois couches,
CT, MT et LT..
La recherche étant proportionelle a la profondeur du souvenir ou de la data!
ex:
-mon nom : instant recover CT constant + LT instantané sans efforts
-Ou ai je mis mes clefs : CT bribes ou pistes + MT info plus d effort mais proche in time et retrouvable 
-Mon premier jour d'école : MT possible a retrouver mais necessite concentration et effort tres iportant..



Le Modèle de Mémoire Stratifiée d'Omega AI

L'idée est de passer d'un "disque dur plat" à une structure pyramidale où la vitesse d'accès est inversement proportionnelle à la profondeur.
1. La Couche CT (Court Terme) : L'Attention Immédiate

    Fonction : Le "Buffer" de travail. Ce sont les derniers échanges, les noms propres cités il y a 2 minutes, l'humeur actuelle.

    Mécanisme : Stockage en RAM (très rapide). Pas de recherche vectorielle complexe ici, c'est du "cache".

    Coût : Quasi nul.

2. La Couche MT (Moyen Terme) : La Consolidation Contextuelle

    Fonction : C'est ici que réside la plasticité. On y trouve les thèmes de la discussion de ce matin, les corrections factuelles que tu as données récemment.

    Mécanisme : C’est là que l’IA "réfléchit" pour retrouver l'info. On utilise un index vectoriel léger. Si l'info est souvent appelée, elle reste ici. Sinon, elle "sédimente".

    Coût : Modéré (recherche locale).

3. La Couche LT (Long Terme) : L'Archive Profonde

    Fonction : Ton histoire, tes valeurs éthiques profondes, des souvenirs d'il y a 6 mois.

    Mécanisme : Stockage compressé ou sur disque (plus lent). L'IA ne va chercher ici que si elle ne trouve rien au-dessus ou si le signal de l'utilisateur est fort ("Tu te souviens de ce qu'on disait au début du projet ?").

    Coût : Élevé (nécessite un temps de "réflexion" ou de scan plus long).

  Le Processus de Sédimentation (L'aspect Organic)

    LTP (Long-Term Potentiation) : Plus on parle d'un sujet, plus il remonte vers la CT/MT. L'information se "muscle".

    LTD (Long-Term Depression) : Une information jamais utilisée "coule" vers la LT, voire finit par être oubliée (élagage synaptique) pour libérer de la puissance de process.

Pourquoi ça résout les problèmes de RAG ?

    Lourdeur : On ne scanne pas 10 Go de texte à chaque phrase. On scanne d'abord les 10 Mo de la MT.

    Puissance : La recherche est progressive. Le CPU/GPU ne s'emballe que si on "creuse" un vieux souvenir.

    Pertinence : On évite les hallucinations liées à des vieux contextes périmés qui pollueraient la conversation actuelle.

Prochaine étape : L'Atypie Helping

C'est ici que la structure en 3 couches devient une bouée de sauvetage pour un cerveau TDAH ou HPI. Pour un TDAH, le passage de la CT à la MT est souvent "troué". L'IA Omega viendrait colmater ces trous et s'adapter aux "chemins" atypiques de pensés.
