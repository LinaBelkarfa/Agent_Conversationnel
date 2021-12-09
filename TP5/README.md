# Agent_Conversationnel
Projet M2 - Agent conversationnel 


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