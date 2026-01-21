---
title: IA dans les applications Experience Cloud
description: Découvrez comment les applications Experience Cloud utilisent l’IA générative (GenAI), l’Assistant IA et l’IA agentique.
source-git-commit: 0e3839f829efc5670c235435d49ed5e49da2ed13
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 13%

---

# IA dans Experience Cloud

Bienvenue dans le guide complet des fonctionnalités d’IA dans les applications Adobe Experience Cloud. Cette documentation explique comment l’IA générative, l’assistant d’IA et les agents Adobe sont intégrés à vos workflows Experience Cloud pour accélérer la productivité et améliorer la prise de décision.

## Éléments compris dans ce guide

### Assistant IA

[AI Assistant](./ai-assistant/ai-assistant-ui.md) est un outil d’IA intelligent, conversationnel et génératif qui stimulera la productivité et redéfinira le travail dans les applications Adobe Experience Platform. Les utilisateurs peuvent acquérir des connaissances sur les produits, résoudre les problèmes et trouver des informations opérationnelles grâce à des invites en langage naturel. Vous pouvez également utiliser l’assistant AI pour accéder aux agents Adobe Experience Platform et à d’autres fonctionnalités d’IA.

**Fonctionnalités principales :**

- **Interface de conversation** : vous pouvez choisir entre une interface d’affichage plein écran et une interface d’affichage du rail pour répondre aux préférences de votre workflow.
- **Invites de découverte** : l’assistant AI fournit des invites préconfigurées organisées par catégories telles que Apprendre, Analyser et Optimiser.
- **Paramètre de contexte** : vous pouvez configurer les paramètres de l’application, du sandbox et de la vue de données pour recevoir des réponses adaptées à vos besoins.
- **Visualisation des données** : cet outil fournit des graphiques et des diagrammes interactifs, ce qui vous permet d’obtenir des informations à partir de vos données.
- **Vérification de la réponse** : toutes les réponses incluent des citations de la source, des explications du raisonnement de l’IA et des mécanismes permettant de fournir une rétroaction.


### Agent Orchestrator

[Adobe Experience Platform Agent Orchestrator](./agents/agent-orchestrator.md) est la nouvelle couche agentic de Adobe Experience Platform. Conçu pour exploiter la richesse des données et des connaissances clientèle de la plateforme, Experience Platform Agent Orchestrator alimente l’intelligence et le raisonnement d’agents experts spécialement conçus pour Adobe Experience Platform, leur permettant d’exécuter des prises de décision complexes et de résoudre des problèmes à grande vitesse et à grande échelle, le tout sous supervision humaine. Lorsque vous posez des questions ou demandez de l’aide en langage naturel dans une interface conversationnelle telle que l’assistant IA, Agent Orchestrator fait automatiquement appel à des agentes et agents spécialisés pour vous fournir les bonnes réponses. Agent Orchestrator mémorise l&#39;historique de vos conversations, ce qui vous permet de vous appuyer sur les questions précédentes naturellement sans répéter le contexte, et d&#39;associer les informations provenant de plusieurs agents pour vous présenter des réponses claires et unifiées.

**Composants principaux :**

- **Moteur de raisonnement** : crée des plans détaillés et ajuste les approches selon les besoins
- **Agents spécialisés** : agents spécialement conçus pour des tâches et des domaines spécifiques
- **Base de connaissances** : accès sécurisé à la veille économique et à la documentation

### Agents spécialisés

#### Agent Audience

Audience Agent fournit des informations sur les audiences, notamment :

- Détection des modifications importantes de la taille de l’audience.
- Identification des audiences en double.
- Exploration de l’inventaire des audiences.
- Récupération des tailles d’audience.

Lisez la [documentation d’Audience Agent](./agents/audience.md) pour plus d’informations.

#### Data Insights Agent

Disponible dans Customer Journey Analytics, le Data Insights Agent :

- Répond aux questions sur vos données à l’aide du langage naturel.
- Crée des visualisations pertinentes dans Analysis Workspace.
- Utilise des composants de votre vue de données et des données réelles.

#### Agent d’analyse de parcours

L’agent d’analyse de Parcours permet aux utilisateurs de Adobe Journey Optimizer de :

- Analysez et optimisez les parcours à l’aide du langage naturel.
- Détectez et résolvez les conflits de planning ou d’audience.
- Analysez les performances et les points de chute.

Pour plus d’informations[&#x200B; consultez la documentation de Journey Agent &#x200B;](./agents/ajo-agent.md).

#### Agent du support technique du produit

Utilisez l’agent du support produit pour le débogage et le dépannage en libre-service :

- Résolution des problèmes liés aux fonctionnalités de Adobe Experience Platform sans quitter les workflows.
- Créez des tickets d’assistance avec du contexte à partir des interactions de l’assistant AI.
- Vérifiez les mises à jour des tickets via l’assistant AI.

Pour plus d’informations, consultez la [documentation de l’agent d’assistance produit](./agents/product-support.md).

## Prise en main

### Exigences d’accès

Pour utiliser l’assistant AI et les agents Experience Platform, votre administrateur Adobe doit configurer les autorisations appropriées :

- Pour utiliser l’assistant AI dans Real-Time CDP et Adobe Journey Optimizer, vous devez disposer de l’autorisation « Activer l’assistant AI », ainsi que de l’autorisation « Afficher les informations opérationnelles » pour accéder aux questions opérationnelles.
- L’accès à l’assistant d’IA dans Customer Journey Analytics est géré par le biais du contrôle d’accès Customer Journey Analytics, qui vous permet de poser des questions sur les connaissances du produit et les informations sur les données.
- Pour Adobe Experience Manager, vous pouvez accéder à l’assistant AI par le biais d’autorisations définies dans le Adobe Admin Console.

### Confidentialité et sécurité

AI Assistant est conçu avec la confidentialité, la sécurité et la gouvernance au premier plan :

- Aucune donnée personnelle n&#39;est utilisée pour la formation.
- Toutes les politiques de contrôle d’accès existantes sont respectées.
- Conformité à la norme HIPAA en cas d’utilisation avec Adobe Experience Platform Healthcare Shield.
- Politique de rétention de 30 jours pour les logs d’interaction.
- Isolation des données spécifique au sandbox.

## Bonnes pratiques

Pour tirer le meilleur parti de votre expérience d’assistant d’IA, suivez ces bonnes pratiques :

- **Soyez précis** dans vos invites pour obtenir des informations ciblées et pertinentes de la part de l&#39;assistant d&#39;IA.
- **Vérifiez les réponses** en examinant les citations de la source et les explications de raisonnement fournies par l’assistant d’IA.
- **Utilisez le paramètre contextuel** pour vous assurer que les sources de données les plus pertinentes sont utilisées pour vos questions.
- **Faites des commentaires** pour améliorer les performances et la précision de l’assistant d’IA au fil du temps.
- **Combinez les informations** de plusieurs agents pour obtenir une analyse plus complète et mieux équilibrée.

## Considérations juridiques

Lors de l’utilisation de l’assistant d’IA, il est important de tenir compte des principales considérations juridiques et pratiques. Actuellement, l’assistant AI prend uniquement en charge les réponses en anglais. Veillez toujours à vérifier les informations fournies, car les modèles linguistiques peuvent parfois faire des erreurs. Utilisez les étapes de raisonnement et les explications incluses dans les réponses pour mieux comprendre les réponses que vous recevez. Si vous rencontrez des problèmes ou des inexactitudes, envoyez des commentaires pour améliorer l’assistant d’IA au fil du temps.
