[:arrow_left: Retour vers le portfolio](https://github.com/ThibaultLanthiez/Portfolio)

# Prédire le nombre de décès quotidiens dus au Covid-19

Pendant l'été 2020, je me posé la question si un modèle de machine learning pouvait prédire le nombre de décès quotidiens dus au Covid-19. Cela afin de mieux anticiper les évolution posssible de l'épidémie.

J'ai donc téléchargé les données de la situation sanitaire pour chaque pays. Je les ai mis en forme pour pouvoir le analyser puis pour créer des fenêtres de 2 mois. Le modèle renvoie 30 jours de prédictions en fonction de données multivariées (nombre de nouveaux cas quotidiens, nombre de décès quotidiens et nombre de décès cumulés) de 30 jours d'historique.  

Ce modèle est un réseau de neurones récurrents (RNN) développé avec la bibliothèque TensorFlow.Keras en langage Python.

Dans le graphique ci-dessous, l''entraînement et la validation se sont fait sur les données de nombreux pays jusqu'au 19 avril 2020.

Le test a ensuite été effectué sur chaque pays (ici le Royaume-Uni) en donnant l'historique entre le 21 mars et le 19 avril 2020 (30 jours) et en comparant les prédictions et la réalité pour les 30 jours suivants (entre le 20 avril et le 19 juin 2020). On remarque que le modèle arrive bien à prédire la chute du nombre de décès quotidiens bien que ces derniers étaient en forte augmentation.

<img src="https://github.com/ThibaultLanthiez/Prediction-nombre-deces-quotidiens-Covid-19/blob/main/graphique.png" width="140%" and height="120%"/>

# Code

Voici le code du projet : [notebook](https://github.com/ThibaultLanthiez/Prediction-nombre-deces-quotidiens-Covid-19/blob/main/Projet_7_R%C3%A9gression_Covid_19_Time_Series.ipynb)
