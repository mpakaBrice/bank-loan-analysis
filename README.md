# bank-loan-Analysis


🎯 Problématique
La banque All-Life Bank possède une base de clients dont la majorité sont des déposants (épargnants). L'année dernière, la banque a mené une campagne qui a permis de convertir plus de 9% des clients en souscripteurs de prêts personnels.

La problématique centrale de ce dataset :

Comment une banque peut-elle identifier, parmi ses clients épargnants, ceux qui sont les plus susceptibles de souscrire à un prêt personnel, afin d'optimiser l'efficacité de ses campagnes marketing ?
L'objectif de ce projet est de construire un modèle prédictif pour identifier les futurs clients ayant une forte probabilité de souscrire à un prêt, afin de mieux cibler les efforts marketing et d'optimiser le budget de prospection.

📂 Présentation des Données
Le dataset contient les informations de 5 000 clients. Chaque ligne représente un client avec ses caractéristiques démographiques et sa relation avec la banque.

Dictionnaire des variables
| Colonne | Description | Type |
| :--- | :--- | :---: |
| **ID** | Identifiant unique du client | Numérique |
| **Age** | Âge du client (en années) | Numérique |
| **Experience** | Années d'expérience professionnelle | Numérique |
| **Income** | Revenu annuel (en milliers de $) | Numérique |
| **ZIP Code** | Code postal du domicile | Catégoriel |
| **Family** | Taille de la famille du client | Numérique |
| **CCAvg** | Dépense moyenne mensuelle sur carte de crédit ($) | Numérique |
| **Education** | Niveau d'études (1: Bachelor, 2: Graduate, 3: Prof.) | Catégoriel |
| **Mortgage** | Valeur de l'hypothèque immobilière ($) | Numérique |
| **Personal Loan** | Le client a-t-il accepté le prêt ? (**Cible**) | Binaire (0/1) |
| **Securities Account** | Possède un compte-titres ? | Binaire (0/1) |
| **CD Account** | Possède un certificat de dépôt ? | Binaire (0/1) |
| **Online** | Utilise les services bancaires en ligne ? | Binaire (0/1) |
| **CreditCard** | Utilise une carte de crédit All-Life Bank ? | Binaire (0/1) |


🛠️ Étapes de l'Analyse

Nettoyage (Data Cleaning) :

Vérifier les valeurs manquantes.

Corriger les valeurs aberrantes (ex: l'expérience négative présente dans ce dataset).

Analyse Exploratoire (EDA) :

Quelle est la distribution des revenus selon l'acceptation du prêt ?

Le niveau d'éducation influence-t-il la décision ?

Visualisation : Utilisation de Seaborn et Matplotlib pour identifier les corrélations.

🚀 Comment utiliser ce projet

git clone https://github.com/mpakaBrice/bank-loan-analysis.git

pandas, seaborn, matplotlib, scikit-learn.

Le dataset est accessible directement via l'URL Hugging Face.

Les difficultés

🔄 Reconversion professionnelle

🚀 Motivé et en apprentissage continu
