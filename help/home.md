---
title: L’IA dans les applications Experience Cloud
description: Découvrez comment les applications Experience Cloud utilisent l’IA générative (GenAI), l’assistant d’IA et l’IA dédiée aux agences.
source-git-commit: 58cce845f525e7762f32379a8db5791b677ae54f
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# L’IA dans Experience Cloud

Bienvenue dans le guide complet des fonctionnalités d’IA dans les applications Adobe Experience Cloud. Cette documentation explique comment l’IA générative, l’assistant d’IA et les agents Adobe sont intégrés à vos workflows Experience Cloud pour accélérer la productivité et améliorer la prise de décision.

## Éléments compris dans ce guide

### Assistant IA

[AI Assistant](./ai-assistant/ai-assistant-ui.md) est un outil d’IA intelligent, conversationnel et génératif qui stimulera la productivité et redéfinira le travail dans les applications Adobe Experience Platform. Les utilisateurs peuvent acquérir des connaissances sur les produits, résoudre les problèmes et trouver des informations opérationnelles grâce à des invites en langage naturel. Vous pouvez également utiliser l’assistant AI pour accéder aux agents Adobe Experience Platform et à d’autres fonctionnalités d’IA.

**Fonctionnalités principales :**

- **Interface de conversation** : options d’affichage plein écran et par rail pour différentes préférences de workflow
- **Invites de découverte** : invites préconfigurées organisées par catégorie (Apprendre, Analyser, Optimiser)
- **Paramètre de contexte** : configurez les paramètres de l’application, du sandbox et de la vue de données pour les réponses ciblées
- **Visualisation des données** : graphiques et diagrammes interactifs pour obtenir des informations sur les données
- **Vérification de la réponse** : citations de Source, explications de raisonnement et mécanismes de retour d’informations

### Agent Orchestrator

[Adobe Experience Platform Agent Orchestrator](./agents/agent-orchestrator.md) est la nouvelle couche agentic de Adobe Experience Platform. Conçu pour exploiter les données riches et les connaissances des clients de la plateforme, Experience Platform Agent Orchestrator alimente l&#39;intelligence et la logique derrière des agents Adobe Experience Platform experts spécialement conçus, leur permettant d&#39;exécuter des tâches complexes de prise de décision et de résolution de problèmes à vitesse et à l&#39;échelle, le tout avec une supervision humaine. Lorsque vous posez des questions ou demandez de l’aide en langage naturel dans une interface de conversation comme l’assistant d’IA, Agent Orchestrator fait automatiquement appel à des agents spécialisés pour vous obtenir les bonnes réponses. Agent Orchestrator mémorise l&#39;historique de vos conversations, ce qui vous permet de vous appuyer sur les questions précédentes naturellement sans répéter le contexte, et d&#39;associer les informations provenant de plusieurs agents pour vous présenter des réponses claires et unifiées.

**Composants principaux :**

- **Moteur de raisonnement** : crée des plans détaillés et ajuste les approches selon les besoins
- **Agents spécialisés** : agents spécialement conçus pour des tâches et des domaines spécifiques
- **Base de connaissances** : accès sécurisé à la veille économique et à la documentation

### Agents spécialisés

#### Audience Agent

Fournit des informations sur les audiences, notamment :

- Détection des modifications importantes de la taille de l’audience
- Identification des audiences en double
- Explorer l’inventaire des audiences
- Récupération des tailles d’audience

#### Data Insights Agent

Disponible dans Customer Journey Analytics, cet agent :

- Répond aux questions sur vos données en utilisant le langage naturel
- Génère des visualisations pertinentes dans Analysis Workspace
- Utilise les composants de votre vue de données et des données réelles

#### Journey Agent

Permet aux utilisateurs de Journey Optimizer de :

- Analyse et optimisation des parcours à l’aide du langage naturel
- Détecter et résoudre les conflits de planification ou d’audience
- Analyse des performances et des points de chute

#### Agent du support technique du produit

Offre un débogage et un dépannage en libre-service :

- Résolution des problèmes liés aux fonctionnalités de Adobe Experience Platform sans quitter les workflows
- Créer des tickets d’assistance avec du contexte à partir des interactions de l’assistant AI
- Vérifier les mises à jour des tickets via l’assistant AI

## Prise en main

### Exigences d’accès

Pour utiliser l’assistant AI et les agents Experience Platform, votre administrateur Adobe doit configurer les autorisations appropriées :

- **Real-Time CDP et Adobe Journey Optimizer** : nécessite l’autorisation « Activer l’assistant IA » et l’autorisation « Afficher les informations opérationnelles » pour les questions opérationnelles
- **Customer Journey Analytics** : accès via le contrôle d’accès Customer Journey Analytics pour les questions sur la connaissance des produits et les informations sur les données
- **Adobe Experience Manager** : accès via Adobe Admin Console

### Confidentialité et sécurité

AI Assistant est conçu avec la confidentialité, la sécurité et la gouvernance au premier plan :

- Aucune donnée personnelle n&#39;est utilisée pour la formation
- Toutes les politiques de contrôle d’accès existantes sont respectées
- Conformité à la norme HIPAA en cas d’utilisation avec Adobe Experience Platform Healthcare Shield
- politique de rétention de 30 jours pour les journaux d’interactions
- Isolation de données spécifique au sandbox

## Bonnes pratiques

- **Soyez précis** dans vos invites pour obtenir des informations ciblées
- **Vérifier les réponses** en utilisant les citations de la source et les explications du raisonnement
- **Utilisez le paramètre de contexte** pour garantir des sources de données pertinentes.
- **Fournir des commentaires** pour améliorer les performances de l’assistant d’IA
- **Combiner les informations** de plusieurs agents pour une analyse complète

## Considérations juridiques

- L’assistant AI prend actuellement en charge l’anglais uniquement
- Vérifiez toujours les réponses car les modèles de langue peuvent faire des erreurs
- Revoir les étapes de raisonnement et les explications fournies
- Envoyez vos commentaires en cas de problèmes ou d’inexactitudes

Ce guide fournit tout ce dont vous avez besoin pour utiliser efficacement les fonctionnalités d’IA dans vos applications Experience Cloud, des interactions de base à l’orchestration d’agent avancée en passant par les workflows spécialisés.

