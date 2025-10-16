---
title: Présentation des compétences de l’agent Parcours Analyze et guide de l’utilisateur
description: Guide complet sur la compétence d’analyse de l’agent Journey, qui permet aux utilisateurs et aux utilisatrices d’analyser les parcours marketing, de détecter les problèmes, d’obtenir des informations et d’optimiser l’engagement de la clientèle.
solution: Journey Optimizer
product: journey optimizer
role: Admin,User,Developer,Leader
source-git-commit: 26b579471b591d3c436f4275d07303d297e0fbf8
workflow-type: tm+mt
source-wordcount: '979'
ht-degree: 38%

---


# Agent Parcours Analyze : présentation des compétences et guide de l’utilisateur

## Vue d’ensemble

Journey Agent permet aux utilisateurs de Journey Optimizer d’analyser et d’optimiser les parcours à l’aide d’une interface en langage naturel. Avec Journey Agent, les utilisateurs et utilisatrices peuvent rapidement identifier et résoudre les conflits de planning et/ou d’audience, détecter les points d’abandon d’utilisateur ou d’utilisatrice dans un parcours et fournir des informations ou des recommandations. Il permet aux personnes professionnelles de prendre des décisions fondées sur des données, d’améliorer l’engagement de la clientèle et de rationaliser l’orchestration de parcours.

Découvrez l’agent en un coup d’œil et en savoir plus dans cette [présentation](https://experienceleague.adobe.com/fr/slides/journey-agent-overview).

>[!AVAILABILITY]
>
>Le Journey Agent est disponible pour tous les clients qui ont accès à l’assistant AI. Toutefois, vous aurez besoin des autorisations suivantes pour utiliser pleinement les fonctionnalités de Journey Agent :
>
>**Afficher les Parcours** : cette autorisation vous permet d’afficher des informations sur le parcours directement dans l’assistant AI.
>
>**Gérer les Parcours** : l’autorisation À vous permet de créer des parcours directement dans l’assistant AI.
>
>**Afficher les segments** : cette autorisation vous permet d’afficher des informations sur les audiences directement dans l’assistant AI.
>
>**Gérer les segments** : pour obtenir l’autorisation, vous pouvez créer de nouvelles audiences directement dans l’assistant AI.

![Exemple pour AJO Agent](./images/ajo-agent/ajo-agent-sample.png)

## Cas d’utilisation

### Principaux cas d’utilisation de l’analyse de l’agent Journey

La compétence d’analyse de l’agent Journey offre diverses fonctionnalités qui peuvent être utilisées pour optimiser les efforts marketing :

1. **Analyse des abandons de parcours**

   - Identifiez où et pourquoi les clients et clientes abandonnent leur parcours.
   - Détectez des modèles dans le comportement de la clientèle qui conduisent à leur désengagement.
   - Utilisez les informations pour affiner la conception des parcours et améliorer la fidélisation.

1. **Analyse du chevauchement d’audiences dans les parcours**

   - Analysez le chevauchement d’audiences dans plusieurs parcours.
   - Évitez la lassitude de l’audience causée par un ciblage excessif.
   - Optimisez la segmentation pour garantir un engagement équilibré.

1. **Analyse du chevauchement de plannings dans les parcours**

   - Détectez les conflits d’horaires entre les parcours planifiés ciblant la même audience.
   - Évitez les excès de communication et améliorez l’efficacité de la planification.
   - Maximisez l’impact sur l’audience en veillant à ce que les parcours se déroulent à des heures optimales.

1. **Informations opérationnelles**

   - Informations sur les Parcours basés sur des invites - Informations opérationnelles de surface sur les parcours , c’est-à-dire « Afficher tous les parcours en direct ».

Pour chacune de ces analyses, l’agent détecte non seulement les problèmes, mais fournit également des recommandations **exploitables pour les résoudre**.


## Compétences incluses dans le champ d’application et hors du champ d’application

### **Dans le champ d’application**

Les capacités suivantes sont prises en charge par l’analyse de l’agent Journey :

- **Requêtes réactives** : permet aux utilisateurs et aux utilisatrices de poser des questions spécifiques sur les performances du parcours, l’utilisation de l’audience et les conflits de planning.
- **Intégration à d’autres agents** : collabore avec l’agent Audience et l’agent Data Insights pour une analyse plus approfondie.
- **Structuration de la réponse de l’agent** : raisonnement (expliquer la logique), résumé de l’analyse (mettre en évidence les points clés), détails du problème (décrire le problème) et recommandation (proposer les étapes suivantes).

### **Hors du champ d’application**

Les fonctionnalités suivantes ne sont pas prises en charge actuellement :

- **Création automatisée de parcours**
- **Détection des anomalies en temps réel**
- **Chevauchement des canaux**
- **Analyse de l’entrée de parcours**
- **Analyse des problèmes techniques**
- **Analyse de la lassitude**

## Exemples de prompt

### Prompts courants pour l’analyse des parcours

Voici des exemples de prompts utiles que les utilisateurs et utilisatrices peuvent utiliser pour explorer, surveiller et dépanner leurs parcours.

### Questions sur le cycle de vie des parcours

- « Quand [Nom du Parcours ] a-t-il été publié ? »
- « Quand [Nom du Parcours a-t-il été arrêté ] ? »
- « Répertorier tous les parcours actuellement en mode test »

### Questions sur les ressources des parcours

- « Combien de parcours en direct ai-je ? »
- « Donnez-moi la liste de tous les parcours récurrents planifiés et de leurs durées d’exécution prévues. »

### Informations sur les audiences et les parcours

- « Quelles audiences sont utilisées dans plus de X parcours ? »
- « Répertoriez tous les parcours à l’aide de l’audience [nom de l’audience]. »

### Analyse des abandons

- « Je souhaite analyser les abandons par nœud pour la campagne du 4 juillet par parcours. »
- « Effectuez une analyse des abandons pour la campagne du 4 juillet par parcours. »
- « Qu&#39;est-ce que la perte de profil au cours de la campagne du parcours du 4 juillet ? »
- « Indique l’endroit où les utilisateurs quittent la campagne du 4 juillet dans le parcours. »

### Prompts d’analyse des conflits

Utilisez ces prompts pour analyser les conflits potentiels entre les parcours, y compris les chevauchements de plannings et d’audiences :

- « Pouvez-vous effectuer une analyse complète des conflits pour notre parcours [Nom du Parcours ] avec des informations de type conflit (planification/audience) avec des parcours actifs/en cours d’exécution ? »
- « Veuillez effectuer une analyse des conflits de planification pour le parcours [Nom du Parcours ] avec des informations sur le type de conflit. »
- « Veuillez effectuer une analyse du chevauchement des audiences pour le parcours [Nom du Parcours ] avec des informations de type conflit. »
- « Y a-t-il des conflits de planification pour le parcours [Nom du Parcours ] ? »
- « Afficher les conflits de chevauchement d’audience pour le parcours [Nom du Parcours ]. »
- « Analyser tous les conflits pour le nom du parcours [Parcours ] avec d’autres parcours dynamiques. »
- « Quels sont les conflits actuels pour le parcours [Nom du Parcours ] ? »
- « Vérifiez si le parcours [Nom du Parcours ] présente des conflits d’audience avec d’autres parcours. »
- « Recherchez les conflits de planification impliquant le parcours [Nom du Parcours ]. »
- « Je souhaite être informé de tous les conflits de parcours pour [Nom du Parcours ]. »
- « Y a-t-il des parcours en direct en conflit avec [Nom du Parcours ] par planning ou audience ? »
- « Identifier les types de conflit pour le parcours [Nom du Parcours ] par rapport à l’exécution de parcours. »
- « Affichez les audiences qui se chevauchent pour le parcours [Nom du Parcours ] et d’autres parcours. »
- « Mettez en évidence les chevauchements de planification entre le nom de parcours [Parcours ] et les parcours en direct. »
- « Le parcours [Nom du Parcours ] est-il en conflit avec un autre parcours ? »
- « Veuillez détecter et répertorier les conflits pour le nom de Parcours []. »
- « Signaler tous les types de conflits pour le parcours [Nom du Parcours ]. »
- « Donnez-moi une répartition des conflits (planification et audience) pour [Nom du Parcours ]. »
- « [Nom du Parcours ] a-t-il des conflits qui peuvent affecter les performances ? »
- « Existe-t-il des conflits actifs affectant [Nom du Parcours ] ? »
- « Répertorier les parcours en conflit avec le nom du Parcours [] par planning ou audience. »
- « Le parcours [Nom du Parcours ] a-t-il déclenché des alertes de conflit ? »
- « Recherchez des conflits d’audience potentiels pour le parcours [Nom du Parcours ]. »
- « Analyse du risque de conflit pour le parcours [Nom du Parcours ]. »
- « Fournissez des diagnostics de conflit pour [Nom du Parcours ]. »

## Bonnes pratiques

### Bonnes pratiques en matière de prompt

Pour maximiser l’efficacité de l’analyse de l’agent Journey, suivez ces bonnes pratiques :

1. **Être précis** : utilisez des questions claires et concises pour obtenir des informations ciblées. Par exemple, au lieu de demander « Quels sont mes parcours ? », indiquez « Répertorier tous les parcours créés le mois dernier ».
1. **Combiner les informations** : intégrez les informations de l’agent Audience et de l’agent Data Insights pour obtenir une vue d’ensemble des performances des parcours.
1. **Affinage itératif** : utilisez l’analyse des abandons et des chevauchements pour affiner de manière itérative la conception et le planning des parcours.

### Bonnes pratiques de configuration

- **Définir des objectifs clairs** : avant d’analyser les parcours, définissez des objectifs clairs (par exemple, améliorer la fidélisation, augmenter les conversions).
- **Contrôler régulièrement** : planifiez des vérifications régulières des performances des parcours afin d’identifier les tendances et les anomalies.
- **Optimiser la segmentation** : veillez à ce que la segmentation de l’audience soit équilibrée afin d’éviter la lassitude et de maximiser l’engagement.

