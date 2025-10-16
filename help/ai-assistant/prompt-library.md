---
title: Bibliothèque d’invites de l’assistant AI
description: Découvrez les différents types d’invites et de modèles d’invites que vous pouvez utiliser lors de l’interrogation de l’assistant AI.
source-git-commit: 4bb6da3fe1abee98446df62c94730274e0931493
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 3%

---

# Bibliothèque d’invites de l’assistant AI

Lisez ce guide pour connaître les différents types d’invites que vous pouvez utiliser sur l’assistant AI.

## Agent Audience

Les sections suivantes fournissent des exemples d’invites que vous pouvez utiliser avec l’Audience Agent pour explorer et analyser vos audiences. Il s’agit notamment de moyens d’étudier les caractéristiques des audiences, de détecter les audiences en double, de récupérer les tailles d’audience et de surveiller les changements significatifs de la taille d’audience au fil du temps. Utilisez ces invites pour obtenir des informations plus précises et maintenir la qualité des données de votre audience.

### Exploration des audiences de conversation

- « Afficher les champs pour les acheteurs aisés. »
- « Quelles audiences n’ont été activées ou utilisées dans aucune campagne au cours des 30 derniers jours ? »
- « Répertoriez toutes les audiences qui ont été mappées à de nouvelles destinations au cours des 3 derniers mois. »

### Détecter les audiences en double

- « Existe-t-il des audiences avec des descriptions identiques ou similaires ? »
- « Identifiez les audiences qui ont les mêmes règles, mais des noms différents. »
- « Montrez-moi toutes les audiences qui ont les mêmes règles, mais des destinations d’activation différentes. »

### Récupérer la taille de l’audience

- « Quelle est la taille actuelle de mon audience « Membres Gold Star en California_f153e1 » ? »
- « Quel est mon public le plus important ? »

### Détecter les modifications importantes de la taille de l’audience

- « Quelles audiences ont augmenté leur taille de plus de 20 % au cours de la dernière semaine ? »
- « Quelles audiences ont vu leur taille diminuer de plus de 15 % au cours du dernier mois ? »
- « Quel est mon public qui croît le plus rapidement ? »

## Data Insights Agent

Les exemples d’invites ci-dessous peuvent être utilisés avec Data Insights Agent pour analyser vos données, identifier les tendances et découvrir des informations exploitables.

### Visualisation des données

- « Montrez-moi les bénéfices en septembre. »
- « Tendance des commandes en septembre. »
- « Afficher le chiffre d’affaires par région en septembre. »
- « Part du chiffre d’affaires par catégorie de produits. »
- « Commandes par jour de la semaine, de janvier à mai. »
- « Afficher les commandes par genre, de mars à juin. »
- « Quel est le bénéfice sur l’ensemble des SKU de février à mai ? »
- « Chiffre d’affaires par nom de magasin en septembre. »
- « Quels étaient mes 10 principaux SKU en termes de profit en septembre ? »
- « Proportion des achats par mois de l’année. »
- « Bénéfice total en septembre. »

## Journey Agent

Les exemples d’invites ci-dessous peuvent être utilisés avec Journey Agent pour vous aider à analyser les cycles de vie des parcours, à gérer les ressources de parcours, à obtenir des informations sur les relations entre l’audience et le parcours et à détecter les conflits entre les parcours. Utilisez ces invites pour optimiser l&#39;orchestration des parcours et résoudre les problèmes efficacement.

### Questions sur le cycle de vie des parcours

- « Quand a-t-{JOURNEY_NAME} été publié ? »
- « Quand a-t-{JOURNEY_NAME} été arrêté ? »
- « Répertorier tous les parcours actuellement en mode test »

### Questions sur les ressources des parcours

- « Combien de parcours en direct ai-je ? »
- « Donnez-moi la liste de tous les parcours récurrents planifiés et de leurs durées d’exécution prévues. »

### Informations sur les audiences et les parcours

- « Quelles audiences sont utilisées dans plus de X parcours ? »
- « Répertoriez tous les parcours utilisant l’audience {AUDIENCE_NAME}. »

### Prompts d’analyse des conflits

Utilisez ces prompts pour analyser les conflits potentiels entre les parcours, y compris les chevauchements de plannings et d’audiences :

+++Sélectionner pour afficher la liste

- « Pouvez-vous effectuer une analyse complète des conflits pour notre {JOURNEY_NAME} de parcours avec des informations de type conflit (planification/audience) avec des parcours actifs/en cours d’exécution ? »
- « Veuillez effectuer une analyse des conflits de planification pour les {JOURNEY_NAME} de parcours avec des informations de type conflit. »
- « Veuillez effectuer une analyse du chevauchement des audiences pour les {JOURNEY_NAME} de parcours avec des informations de type conflit. »
- « Existe-t-il des conflits de planification pour les {JOURNEY_NAME} de parcours ? »
- « Afficher les conflits de chevauchement d’audience pour les {JOURNEY_NAME} de parcours. »
- « Analysez tous les conflits pour les {JOURNEY_NAME} de parcours avec d’autres parcours actifs. »
- « Quels sont les conflits actuels pour les {JOURNEY_NAME} de parcours ? »
- « Vérifiez si le parcours {JOURNEY_NAME} présente des conflits d’audience avec d’autres parcours. »
- « Recherchez les conflits de planification impliquant des {JOURNEY_NAME} de parcours. »
- « Je veux être au courant de tous les conflits de parcours pour {JOURNEY_NAME}. »
- « Y a-t-il des parcours en direct qui entrent en conflit avec {JOURNEY_NAME} par planning ou audience ? »
- « Identifiez les types de conflit pour les {JOURNEY_NAME} de parcours par rapport aux parcours en cours d’exécution. »
- « Afficher des audiences qui se chevauchent pour les {JOURNEY_NAME} de parcours et d’autres parcours. »
- « Mettez en évidence les chevauchements de planification entre les {JOURNEY_NAME} de parcours et les parcours en direct. »
- « Le parcours {JOURNEY_NAME} est-il en conflit avec un autre parcours ? »
- « Veuillez détecter et répertorier les conflits pour les {JOURNEY_NAME}. »
- « Signalez tous les types de conflits pour les {JOURNEY_NAME} de parcours. »
- « Donnez-moi une répartition des conflits (planification et audience) pour {JOURNEY_NAME}. »
- « Existe-t-{JOURNEY_NAME} des conflits susceptibles d’affecter les performances ? »
- « Existe-t-il des conflits actifs affectant {JOURNEY_NAME} ? »
- « Répertorier les parcours en conflit avec {JOURNEY_NAME} par planning ou audience. »
- « parcours {JOURNEY_NAME} a-t-il déclenché des alertes de conflit ? »
- « Rechercher des conflits d’audience potentiels pour les {JOURNEY_NAME} de parcours. »
- « Analysez le risque de conflit pour les {JOURNEY_NAME} de parcours. »
- « Fournir des diagnostics de conflit pour {JOURNEY_NAME}. »

+++

## Agent du support technique du produit

L’agent d’assistance produit vous aide à résoudre les problèmes, à créer des cas d’assistance et à suivre le statut de vos tickets d’assistance. Utilisez les exemples d’invites suivants pour obtenir de l’aide.

### Aide au dépannage

- « Pourquoi le nombre de profils diffère-t-il sur le tableau de bord d’utilisation des licences et la page d’accueil d’Experience Platform ? »
- « Quelles sont les raisons pour lesquelles un parcours ne se déclenche pas ? »
- « Comment Adobe Experience Platform crée-t-il des expériences en temps réel ? »
- « Comment configurer et utiliser les alertes dans Adobe Experience Platform ? »
- « Quelle est la limite pour les tâches de segmentation par lots dans l’activation de Adobe Experience Platform ? »
- « Quelle est la limite de richesse moyenne des profils dans l’activation de Adobe Experience Platform ? »

### Création de dossier d’assistance

- « Créez un ticket d’assistance. »
- « Pouvez-vous m’aider à créer un ticket d’assistance ? »

### Suivre la progression du cas

- « Quelles sont les dernières informations sur mon dossier E-12345 ? »
- « Quelle est la mise à jour sur le ticket E-67890 ? »

