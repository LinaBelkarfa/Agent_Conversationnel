# Agent_Conversationnel
Projet M2 - Agent conversationnel (rassemble tous les TP de l'année)


<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#tp1">TP1 - Agents basics </a></li>
      </ul>
      <ul>
        <li><a href="#tp2">TP2 - ChatBot DataCamp </a></li>
      </ul>
       <ul>
        <li><a href="#tp3">TP3 - Eliza </a></li>
      </ul>
      <ul>
        <li><a href="#tp4">TP4 - Parry </a></li>
      </ul>
      <ul>
        <li><a href="#tp5">TP5 - GUS </a></li>
      </ul>
    </li>
    <li>
      <a href="#conclusions">Conclusions</a>
      <ul>
        <li><a href="#problèmes">Problèmes</a></li>
      </ul>
      <ul>
        <li><a href="#améliorations-possibles">Améliorations possibles</a></li>
      </ul>
    </li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project
Enoncé : travaux effectués pendant les cours, avec en plus votre apport personnel  +  rapport avec mode d'emploi de votre rendu 

### TP1
#### Etude des types fondamentaux d'agents intelligents.

Quatre types fondamentaux, du plus simple au plus général :
* Agents réflexes simples
* Agents réflexes fondés sur des modèles (ou avec état interne), ce sont des agents qui conserventune trace du monde
* Agents fondés sur des buts
* Agents fondés sur l'utilité

Dans ce TP est réalisé : 
* Un agent réflexes simples
* Un agents réflexes avec état interne
* Un agent réflexe avec état interne et but
De plus, une tentative de prendre en compte les distances entre les salles n'a pas été terminé. 
Cela aurait permi de donner un but plus difficile que "nettoyer toutes les salles". Par exemple, le nouveau but aurait été "nettoyer toutes les salles en parcourant le moins de distance possible"

Il s'agit d'un fichier .ipynb (jupyter notebook, Python3), ce qui permet d'y voir les commentaires et détails d'exécutions.
C'est donc dans ce ipynb que tous les détails de mes réalisations se trouvent.

### TP2
#### Ce TP est une réalisation tiré du tutoriel de Datacamp "Building Chatbots in Python", chapitre 1 "Chatbots 101".
Lien du tuto : https://app.datacamp.com/learn/courses/building-chatbots-in-python 

* Il s'agit là d'une première utilisation d'ELIZA. 
* ELIZA est, en intelligence artificielle, un programme informatique écrit par Joseph Weizenbaum entre 1964 et 1966, qui simule un psychothérapeute rogérien en reformulant la plupart des affirmations du « patient » en questions, et en les lui posant.
* ELIZA fonctionne par reconnaissance de formes et substitution des mots-clés dans les phrases produites. Typiquement, une affirmation « A » peut recevoir en retour la question « Pourquoi dites-vous que A ? ».

Ce TP est donc une introduction à la réalisation et à l'utilisation des agents intelligents, notamment ELIZA.
Il est réalisé en .ipynb (Jupyter Notebook, Python3), ce qui permet d'en voir les commentaires et détails d'exécutions. 
 
### TP3
#### Dans ce TP nous allons utiliser une réalisation du chatbot Eliza en Python, mise à disposition par sondéveloppeur avec une Licence MIT.
Lien du repo : https://github.com/wadetb/eliza 

#### Questions
 1. Ajoutez d'autres règles au script pour rendre le chatbot encore plus convaincant.
 2. Penser à un scénario de conversation par exemple, voyage, cuisine, musique, et ajouter des règles au script pour soutenir une conversation dans ce scénario.
 3. What is your name? ne se comporte pas comme What is your name ? Modifiez le code python pour éviter ce problème.
 4. Modifiez le code pour qu'Eliza se rende compte s'il utilisateur ré^ète les mêmes phrases et gérez correctement cette situation. Par exemple qu'Eliza dise "Stop repeting yourself". Utilisez la distance de Levenshtein pour comparer deux phrases ( exemple : what is your name? What's your name ? your name ? , se ressemblent)
 5. Remplacez les mot clés dans (Clé, Patron, Règle de transformation) par des regexp. 
 6. Modifiez les script pour exploiter les regexp.
 7. Pensez à rédiger un document décrivant la démarche que vous avez suivie, votre apport personnel et vos éventuelles remarques. Cette documentation sera intégrée à votre rapport final. 


Ce TP est réalisé en .ipynb (Jupyter Notebook, Python3), ce qui permet d'en voir les commentaires et détails d'exécutions. 

 

### TP4
#### Dans cette séance, vous devez créer un nouveau chatbot, ayant certaines caractéristiques de Parry.

#### Travail à faire
Pour la création de Parry, vous pouvez vous baser sur le code utilisé pour programmer Eliza et l'adapter sur les points suivants :
  1. Ajouter les trois variables affectives (peur, colère et méfiance),
  2. Avant de traiter la phrase tapée par l'utilisateur, vous devrez l'analyser et modifier les valeurs des trois variables affectives, en conséquence.
  3. Vous devrez mettre au point la fonctionalité de sélection de la stratégie de réponse en vous inspirant de l'architecture de Parry vue en cours,
  4. Modifier la syntaxe du script (doctor.txt) pour permettre d'asscocier chaque règle de transformation (reasmb) à une ou plusieurs stratégies : la règle sera alors sélectionnée seulement si elle est associée à la stratégie courante (ex. si la stratégie courante est peur, seules les reasmb associées à peur pourront être sélectionnées).
  5. Modifier le code du chatbot de façon à ce qu'il soit adapté à cette nouvelle syntaxe du script.

Ce TP est réalisé en .ipynb (Jupyter Notebook, Python3), ce qui permet d'en voir les commentaires et détails d'exécutions. 



### TP5
#### Dans cette séance, vous devez créer un GUS organisateur de voyage pour qu'il soit en mesure de faire les réservations demandées par l'utilisateur. 

Vous avez deux possibilités :
* soit (1) de construire votre agent à partir de zéro avec vos choix de structure de données,
* soit (2) d'adapter votre actuelle version d'Eliza, i.e. adapter le script .txt et le code pour qu'il prenne en compte les modifications dans le script. Si vous partez d'Eliza . . . Travail à faire
Il serait préférable que le comportement de l'agent soit parametré grâce à un fichier externe comme c'etait le cas pour Eliza. Ce fichier contiendrait la définition des cadres, de leur slots, etc.

  1. Pensez à modifier le script pour qu'il soit possible de représenter le(s) cadre(s) du GUS. Pensez aussi à modifier le code pour qu'il prenne en compte ces modifications. N'oubliez
pas qu'un cadre peut être hiérarchique i.e. un slot peut avoir un cadre comme valeur. En guise d'exemple, traitez le cas du slot date.
  2. Proposer une solution pour traiter au moins un cas de réponses multiples. Pensez à l'exemple vu en cours d'une réponse concernant plusieurs slots : J'aimerais un vol aller simple de Paris à Nice, avec départ après 17 heures le mardi.

Suggestion : inspirez vous des patrons et des règles de transformation d'Eliza pour extraire les informations des réponses de l'utilisateur et les affecter aux slots appropriés. 

Ce TP est réalisé en .ipynb (Jupyter Notebook, Python3), ce qui permet d'en voir les commentaires et détails d'exécutions. 



### Problèmes rencontrés
* Je n'ai pas eu le temps de terminer le TD4 - Parry 
* Pour TD5 - GUS, j'ai choisi d'utiliser une librarie déjà existante qui permet ce genre de traitement, car nous avions trop de projets en cours à l'heure actuelle, ne me permettant pas de faire dans le détail cette réalisation. La librarie est notamment utilse dans la prise de date de vol.
