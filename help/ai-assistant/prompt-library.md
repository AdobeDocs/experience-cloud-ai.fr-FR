---
title: AI Assistant Prompt Library
description: Learn about the different kinds of prompts and prompt patterns that you can use when querying AI Assistant.
TQID: https://experienceleague.adobe.com/QICjh9cNBT3XeKObkXqSDEGQT26zpv86V36L0tqvSgo
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: dd7883d8eccab3b0f006d55a850248e1c347d7e7
workflow-type: tm+mt
source-wordcount: 813
ht-degree: 17%

---

# AI Assistant Prompt Library

Read this guide for different types of prompts that you can use on AI Assistant.

## Agent Audience

The following sections provide example prompts you can use with the Audience Agent to explore and analyze your audiences. These include ways to investigate audience characteristics, detect duplicate audiences, retrieve audience sizes, and monitor significant changes in audience size over time. Use these prompts to gain deeper insights and maintain the quality of your audience data.

### Conversation audience exploration

- &quot;Show me fields for affluent buyers.&quot;
- &quot;Which audiences have not been activated or used in any campaign in the last 30 days?&quot;
- &quot;List all the audiences that have been mapped to new destinations in the last 3 months.&quot;

### Detect duplicate audiences

- &quot;Do I have any audiences with identical or similar descriptions?&quot;
- &quot;Identify audiences that have the same rules but have different names.&quot;
- &quot;Show me all the audiences that have the same rules but different activation destinations.&quot;

### Retrieve audience size

- &quot;What is the current size of my audience &quot;Gold-star Members in California_f153e1&quot;?&quot;
- &quot;What is my biggest audience?&quot;

### Detect significant changes in audience size

- &quot;Which audiences have increased in size by more than 20% in the last week?&quot;
- &quot;Which audiences have decreased in size by more than 15% in the last month?&quot;
- &quot;What is my fastest growing audience?&quot;

## Data Insights Agent

The following example prompts can be used with the Data Insights Agent to analyze your data, identify trends, and uncover actionable insights.

### Visualisation des données

- &quot;Show me profits in September.&quot;
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

- « Combien de parcours actifs ai-je ? »
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
- &quot;Analyze all conflicts for journey {JOURNEY_NAME} with other live journeys.&quot;
- &quot;What are the current conflicts for journey {JOURNEY_NAME}?&quot;
- &quot;Check if journey {JOURNEY_NAME} has audience conflicts with other journeys.&quot;
- &quot;Check for scheduling conflicts involving journey {JOURNEY_NAME}.&quot;
- &quot;I want to know about all journey conflicts for {JOURNEY_NAME}.&quot;
- &quot;Do any live journeys conflict with {JOURNEY_NAME} by schedule or audience?&quot;
- &quot;Identify conflict types for journey {JOURNEY_NAME} compared to running journeys.&quot;
- &quot;Show overlapping audiences for journey {JOURNEY_NAME} and other journeys.&quot;
- &quot;Highlight scheduling overlaps between journey {JOURNEY_NAME} and live journeys.&quot;
- &quot;Is journey {JOURNEY_NAME} running in conflict with any other journey?&quot;
- &quot;Please detect and list conflicts for {JOURNEY_NAME}.&quot;
- &quot;Report all types of conflicts for journey {JOURNEY_NAME}.&quot;
- &quot;Give me a conflict breakdown (scheduling and audience) for {JOURNEY_NAME}.&quot;
- &quot;Does {JOURNEY_NAME} have any conflicts that may impact performance?&quot;
- &quot;Are there any active conflicts affecting {JOURNEY_NAME}?&quot;
- &quot;List journeys in conflict with {JOURNEY_NAME} by schedule or audience.&quot;
- &quot;Has journey {JOURNEY_NAME} triggered any conflict alerts?&quot;
- &quot;Find potential audience conflicts for journey {JOURNEY_NAME}.&quot;
- &quot;Analyze conflict risk for journey {JOURNEY_NAME}.&quot;
- &quot;Provide conflict diagnostics for {JOURNEY_NAME}.&quot;

+++

## Agent du support technique du produit

The Product Support Agent helps you troubleshoot issues, create support cases, and track the status of your support tickets. Use the following example prompts to get assistance.

### Troubleshooting help

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

