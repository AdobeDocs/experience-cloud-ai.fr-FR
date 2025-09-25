---
title: Adobe Experience Platform Agent Orchestrator
description: En savoir plus sur Adobe Experience Platform Agent Orchestrator.
source-git-commit: c9909616697ef319a307b5c8a1ee135204347844
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---

# Adobe Experience Platform Agent Orchestrator

Adobe Experience Platform Agent Orchestrator est la nouvelle couche d’agent de Adobe Experience Platform. Conçu pour exploiter les données riches et les connaissances des clients de la plateforme, Experience Platform Agent Orchestrator alimente l&#39;intelligence et la logique derrière des agents Adobe Experience Platform experts spécialement conçus, leur permettant d&#39;exécuter des tâches complexes de prise de décision et de résolution de problèmes à vitesse et à l&#39;échelle, le tout avec une supervision humaine. Lorsque vous posez des questions ou demandez de l’aide en langage naturel dans une interface de conversation comme l’assistant d’IA, Agent Orchestrator fait automatiquement appel à des agents spécialisés pour vous obtenir les bonnes réponses. Agent Orchestrator mémorise l&#39;historique de vos conversations, ce qui vous permet de vous appuyer sur les questions précédentes naturellement sans répéter le contexte, et d&#39;associer les informations provenant de plusieurs agents pour vous présenter des réponses claires et unifiées.

Vous pouvez effectuer des workflows complexes de bout en bout par le biais d’une interface conversationnelle intuitive sans avoir à connaître les agents qui travaillent en arrière-plan. Le système comprend vos objectifs, crée des plans détaillés et ajuste son approche selon vos besoins en fonction de vos commentaires. Vous pouvez explorer le panneau de raisonnement pour voir le processus de réflexion étape par étape et mieux comprendre comment vos demandes sont traitées. Avec Agent Orchestrator, vous pouvez vous attaquer à des workflows complexes et optimiser les stratégies dans les applications Adobe Experience Cloud.

Lisez ce document pour en savoir plus sur Agent Orchestrator.

## Composants d’Agent Orchestrator {#components}

Agent Orchestrator se compose de plusieurs éléments essentiels, notamment l’interface conversationnelle de l’assistant d’IA, un moteur de raisonnement pour la prise de décision et la planification, des agents Adobe Experience Platform spécialisés et une base de connaissances qui permet d’accéder aux informations pertinentes.

![Architecture marketing d’Agent Orchestrator.](./images/agent-orchestrator/agentic-architecture.png)

### Interface conversationnelle de l’assistant AI {#ai-assistant}

L’assistant AI est une expérience de conversation que vous pouvez utiliser pour accélérer vos workflows dans les applications Adobe. Vous pouvez utiliser l’assistant d’IA pour mieux comprendre la connaissance des produits, résoudre les problèmes ou rechercher des informations et des informations opérationnelles. AI Assistant prend en charge Experience Platform, Real-Time Customer Data Platform, Adobe Journey Optimizer et Customer Journey Analytics. Vous pouvez utiliser l’assistant AI pour accéder aux agents Experience Platform et à d’autres fonctionnalités d’IA.

Pour plus d’informations, consultez le guide de l’interface utilisateur de l’assistant [AI](../ai-assistant/ai-assistant-ui.md).

### Moteur de raisonnement {#reasoning-engine}

Le moteur de raisonnement interprète vos objectifs en fonction des invites du langage naturel, vérifie les limites ou les exigences et crée des plans détaillés pour vous aider à atteindre vos objectifs. Contrairement aux systèmes simples de questions-réponses, il peut ajuster ses plans à mesure que les choses changent et peut revenir en arrière et essayer différentes approches si nécessaire. Les plans qu’il crée vous sont présentés dans l’interface conversationnelle de l’assistant d’IA. Vous pouvez ainsi voir et suivre le processus, ainsi qu’intervenir si nécessaire.

### Agents Adobe Experience Platform {#agents}

| Agent | Détails | Applications prises en charge |
| --- | --- | --- |
| [Audience Agent](audience.md) | Audience Agent vous permet d’obtenir des informations sur les audiences, notamment la détection des modifications importantes de la taille de l’audience, la détection des audiences en double, l’exploration de l’inventaire de vos audiences et la récupération de la taille de vos audiences. | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> |
| [Data Insights Agent](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/data-analysis-ai) | Data Insights Agent, accessible à partir de l’assistant d’IA dans Customer Journey Analytics, est un agent de conversation d’IA génératif qui répond rapidement et efficacement aux questions sur vos données. Il crée des visualisations pertinentes dans Analysis Workspace à l’aide de composants de votre vue de données et en utilisant vos données réelles. | Customer Journey Analytics |
| Agent d’expérimentation | L’agent d’expérimentation aide les équipes à apprendre plus rapidement en analysant les résultats des expériences, en prédisant l’impact et en proposant de nouvelles expériences. Il centralise les expériences passées et actives afin que vous puissiez tirer parti de ce que vous avez déjà appris, repérer les lacunes et prioriser les prochaines étapes à tester. | Adobe Journey Optimizer Experimentation Accelerator |
| [Journey Agent](./ajo-agent-analyze.md) | Journey Agent permet aux utilisateurs de Adobe Journey Optimizer de créer, d’analyser et d’optimiser des parcours à l’aide d’une interface en langage naturel. Avec Journey Agent, vous pouvez rapidement créer des parcours, détecter et résoudre les conflits de planning ou d’audience, analyser les performances et les points de dépôt, et identifier les parcours les plus performants à répliquer pour les campagnes futures. Il vous permet de prendre des décisions axées sur les données, d’améliorer l’engagement des clients et de rationaliser l’orchestration des parcours. | Adobe Journey Optimizer |
| [Agent du support produit](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/new-features/customer-support) | L’agent de support produit est une fonctionnalité de débogage et de dépannage en libre-service qui vous permet de résoudre les problèmes liés aux fonctionnalités et applications Adobe Experience Platform sans quitter vos workflows. Les administrateurs de l’assistance peuvent créer des tickets d’assistance clientèle avec du contexte à partir de vos interactions avec l’assistant AI et vous pouvez vérifier les mises à jour des tickets via l’assistant AI. | <ul><li>Adobe Experience Platform</li><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li><li>Adobe Journey Optimizer B2B edition</li><li>Customer Journey Analytics</li><li>Adobe Experience Manager</li></ul> |

### Base de connaissances {#knowledge-base}

La base de connaissances fournit aux agents un accès sécurisé à l’intelligence commerciale des clients par le biais de sources de données structurées et non structurées, notamment la documentation du produit Adobe, les métadonnées du client sur les objets commerciaux et les données d’analyse.

## Accès {#access}

Les demandes de l’assistant AI sont authentifiées à l’aide des services Adobe Identity Management. Les autorisations sont appliquées par le contrôle d’accès Adobe Experience Platform et le contrôle d’accès Customer Journey Analytics.

Pour accéder à l’interface conversationnelle de l’assistant AI et utiliser un ou plusieurs agents Experience Platform, votre administrateur Adobe doit vous accorder les autorisations appropriées dans l’interface utilisateur des autorisations ou le Adobe Admin Console :

* **Real-Time CDP** et **Adobe Journey Optimizer** : votre administrateur doit vous accorder l’autorisation **Activer l’assistant AI** pour vous permettre d’accéder à l’assistant AI. Votre administrateur doit également vous accorder les autorisations **Afficher les informations opérationnelles** pour vous permettre de poser des questions relatives aux informations opérationnelles dans l’assistant AI. Les deux autorisations sont définies par l’administrateur dans l’interface utilisateur des autorisations.

* **Customer Journey Analytics** : votre administrateur doit vous accorder l’autorisation d’accéder à l’assistant AI par le biais du contrôle d’accès de [Customer Journey Analytics](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/access-control). Cela vous permet de poser des questions sur la connaissance des produits et les informations sur les données.

>[!NOTE]
>
>Les questions d’informations opérationnelles ne sont pas disponibles pour Customer Journey Analytics. Par conséquent, aucune autorisation supplémentaire ne s’applique.

* **Adobe Experience Manager** : votre administrateur doit vous accorder l’autorisation d’accéder à l’assistant AI via [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html).
