# Agent_Conversationnel
Projet M2 - Agent conversationnel

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

#### Résultats
  1. **Je n'ai pas eu le temps de terminer ce TP**
  2. L'idée était de détecter les insultes grâce à un modele existant qui permet de les cacher, puis détecter les émotions grâce à un autre package
  3. Nous aurions mis à jour les valeurs de nos compteurs peur, colère et méfiance.
  4. En combinant cela à notre liste de mot sensible, nous aurions pu récupérer dans le fichier doctor.txt les reasmb qui renvoie les réactions pour des niveaux différents d'émotions
 
   
