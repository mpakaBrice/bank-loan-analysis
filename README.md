# bank-loan-Analysis

📌 Contexte & Problématique Business:




La banque All-Life Bank souhaite transformer ses clients déposants (comptes épargne) en clients emprunteurs. Lors de la dernière campagne, le taux de conversion n'était que de 9.6%.

Ma mission : Construire un modèle de classification permettant d'identifier les clients ayant la plus forte probabilité d'accepter un prêt personnel.

L'objectif final : Optimiser le budget marketing en ciblant les bons profils et augmenter le taux de transformation global.


📈 Enjeux du Projet

Optimisation du ROI : Réduire les coûts de prospection en ne ciblant que les profils à fort potentiel.

Performance Commerciale : Augmenter le taux de conversion (actuellement à 9,6%).

Expérience Client : Éviter la sollicitation inutile des clients non intéressés pour préserver l'image de la banque.

Aide à la Décision : Fournir une analyse claire des facteurs qui influencent la souscription (Revenus, Éducation, Niveau d'endettement).
<br>
<br>
📂 Présentation des Données
<br>
<br>
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
<br>
<br>
🛠️ Défis Techniques & Solutions :
<br>
<br>
Nettoyage des données incohérentes
<br>
Le défi : La colonne Experience contient des valeurs négatives, ce qui est physiquement impossible.
Ma solution : remplacement par la valeur par 0 plutôt que de supprimer la lignes, afin de conserver la taille de l'échantillon.
<br>
<br>
⚙️ Étapes de l'Analyse 
Nettoyage (Data Cleaning) :

Vérifier les valeurs manquantes.

Corriger les valeurs aberrantes (ex: l'expérience négative présente dans ce dataset).

Analyse Exploratoire (EDA) :

Quelle est la distribution des revenus selon l'acceptation du prêt ?

Le niveau d'éducation influence-t-il la décision ?

Visualisation : Utilisation de Seaborn et Matplotlib pour identifier les corrélations.

Technologies Utilisées
Langage : Python

Librairies : Pandas (Traitement), Seaborn/Matplotlib (Visualisation).
<br>
<br>
💡 Résultats & Recommandations
Facteurs d'influence : Le Revenu annuel et le Niveau d'étude sont les deux prédicteurs les plus puissants.

Recommandation Business : Focaliser les campagnes sur les clients ayant un revenu > $100k et un niveau d'étude "Graduate" ou "Professional".
