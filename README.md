# detection-ddos-par-machine-learning

🛡️ Détection d’attaques DDoS dans les logs de serveurs web

Ce projet vise à détecter automatiquement des attaques DDoS, brute force et autres comportements anormaux dans les journaux de serveurs web à l’aide de techniques de Machine Learning et de Deep Learning.

Il fait partie d’un projet d’analyse de la sécurité réseau et illustre l’utilisation de pipelines ML appliqués aux données de cybersécurité.

📌 Objectifs du projet

Identifier les anomalies dans le trafic réseau.

Détecter les attaques de type DDoS à partir de variables dérivées des logs : fréquence d’accès, taille des requêtes, URLs demandées, code HTTP, etc.

Construire et comparer plusieurs modèles :

Random Forest
Logistic Regression
Réseaux de neuronnes

Fournir un classifieur final robuste et réutilisable.

📊 Jeu de données

Le projet se base sur un dataset public  CIC-DDoS2019, publié par le Canadian Institute for Cybersecurity (CIC).



Prétraitements effectués :

Suppression de la variable ’Unnamed: 0’ et des variables de type Objet : Flow ID, Source IP, Destination IP, Timestamp, SimillarHTTP.
Résultat : 82 variables restantes pour chaque attaque, avec des labels correspondants.


Normalisation des features

Split 70/30 (train/test)



📈 Résultats
Random Forest = modèle le plus performant et le plus stable.
La Régression Logistique reste correcte, mais moins adaptée aux données complexes.
Les Réseaux de Neurones ont montré des limites, liées à une architecture simple



