---
title: Adobe Experience Platform Agent Orchestrator
description: En savoir plus sur Adobe Experience Platform Agent Orchestrator.
source-git-commit: 8c05562121071874002afd6d248f16186616da55
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 13%

---

# Adobe Experience Platform Agent Orchestrator

Adobe Experience Platform Agent Orchestrator est la nouvelle couche agentique d’Adobe Experience Platform. Conçu pour exploiter les données riches et les connaissances des clients d’Experience Platform, Experience Platform Agent Orchestrator alimente l’intelligence et la raison derrière des agents Adobe Experience Platform experts spécialement conçus pour leur permettre d’exécuter des tâches complexes de prise de décision et de résolution de problèmes à grande vitesse et à grande échelle, le tout avec une supervision humaine. Lorsque vous posez des questions ou demandez de l’aide en langage naturel dans une interface conversationnelle telle que l’assistant IA, Agent Orchestrator fait automatiquement appel à des agentes et agents spécialisés pour vous fournir les bonnes réponses. Agent Orchestrator mémorise l&#39;historique de vos conversations, ce qui vous permet de vous appuyer sur les questions précédentes naturellement sans répéter le contexte, et d&#39;associer les informations provenant de plusieurs agents pour vous présenter des réponses claires et unifiées.

Vous pouvez effectuer des workflows complexes de bout en bout par le biais d’une interface conversationnelle intuitive sans avoir à connaître les agents qui travaillent en arrière-plan. Le système comprend vos objectifs, crée des plans détaillés et ajuste son approche selon vos besoins en fonction de vos commentaires. Au cours de votre conversation dans l’assistant d’IA, vous pouvez explorer le panneau de raisonnement d’Agent Orchestrator pour voir le processus de réflexion étape par étape et mieux comprendre comment vos requêtes sont traitées.

>[!SLIDE](agent-orchestrator-overview)

Lisez ce document pour en savoir plus sur Agent Orchestrator.

## Composants d’Agent Orchestrator {#components}

Agent Orchestrator est constitué de plusieurs composants essentiels, notamment l’interface conversationnelle de l’assistant d’IA, un moteur de raisonnement pour la prise de décision et la planification, des agents Adobe Experience Platform spécialisés et une base de connaissances qui permet d’accéder aux informations pertinentes.

![Architecture marketing d’Agent Orchestrator.](./images/agent-orchestrator/agentic-architecture.png)

### Interface conversationnelle de l’Assistant IA {#ai-assistant}

L’assistant AI est une expérience de conversation intelligente en langage naturel qui permet aux utilisateurs des applications Experience Cloud activées d’exploiter les fonctionnalités de GenAI et d’IA dédiée aux agences, dont l’ampleur dépend des applications Experience Cloud sous licence des clients. Pour déverrouiller l’accès, lisez [le guide sur l’accès à l’assistant AI](https://experienceleague.adobe.com/fr/docs/experience-platform/ai-assistant/access).

Pour plus d’informations, consultez le [guide de l’interface d’utilisation de l’Assistant IA](../ai-assistant/ai-assistant-ui.md).

### Moteur de raisonnement {#reasoning-engine}

Le moteur de raisonnement interprète vos objectifs en fonction des invites du langage naturel, vérifie les limites ou les exigences et crée des plans détaillés pour vous aider à atteindre vos objectifs. Contrairement aux systèmes simples de questions-réponses, il peut ajuster ses plans à mesure que les choses changent et peut revenir en arrière et essayer différentes approches si nécessaire. Les plans qu’il crée vous sont présentés dans l’interface conversationnelle de l’assistant d’IA. Vous pouvez ainsi voir et suivre le processus, ainsi qu’intervenir si nécessaire.

### Agents Adobe Experience Platform {#agents}

Les agents Adobe Experience Platform sont un groupe d’agents d’IA dédiés, qualifiés pour fournir des tâches courantes dans les domaines de l’expérience client. Vous trouverez ci-dessous la liste des agents Adobe Experience Platform actuellement disponibles dans les applications Experience Cloud :

| Agent | Détails | Applications prises en charge |
| --- | --- | --- |
| [Audience Agent](audience.md) | Audience Agent vous permet d’obtenir des informations sur les audiences, notamment la détection des modifications importantes de la taille de l’audience, la détection des audiences en double, l’exploration de l’inventaire de vos audiences et la récupération de la taille de vos audiences. | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> |
| [Data Insights Agent](https://experienceleague.adobe.com/fr/docs/analytics-platform/using/cja-overview/cja-b2c-overview/data-analysis-ai) | Data Insights Agent, accessible à partir de l’assistant d’IA dans Customer Journey Analytics, est un agent de conversation d’IA génératif qui répond rapidement et efficacement aux questions sur vos données. Il crée des visualisations pertinentes dans Analysis Workspace en utilisant les composants de votre vue de données et vos données réelles. | Customer Journey Analytics |
| [Agent d’expérimentation](./agent-experiment.md) | L’agent d’expérimentation aide les équipes à apprendre plus rapidement en analysant les résultats des expériences, en prédisant l’impact et en proposant de nouvelles expériences. Il centralise les expériences passées et actives afin que vous puissiez tirer parti de ce que vous avez déjà appris, repérer les lacunes et prioriser les prochaines étapes à tester. | Adobe Journey Optimizer Experimentation Accelerator |
| [Journey Agent](./ajo-agent-analyze.md) | Journey Agent permet aux utilisateurs de Adobe Journey Optimizer de créer, d’analyser et d’optimiser des parcours à l’aide d’une interface en langage naturel. Avec Journey Agent, vous pouvez rapidement créer des parcours, détecter et résoudre les conflits de planning ou d’audience, analyser les performances et les points de dépôt, et identifier les parcours les plus performants à répliquer pour les campagnes futures. Il vous permet de prendre des décisions axées sur les données, d’améliorer l’engagement des clients et de rationaliser l’orchestration des parcours. | Adobe Journey Optimizer |
| [Agent du support produit](product-support.md) | L’agent de support produit est une fonctionnalité de débogage et de dépannage en libre-service qui vous permet de résoudre les problèmes liés aux fonctionnalités et applications Adobe Experience Platform sans quitter vos workflows. Les administrateurs de l’assistance peuvent créer des tickets d’assistance clientèle avec du contexte à partir de vos interactions avec l’assistant AI et vous pouvez vérifier les mises à jour des tickets via l’assistant AI. | <ul><li>Adobe Experience Platform</li><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li><li>Adobe Journey Optimizer B2B edition</li><li>Customer Journey Analytics</li><li>Adobe Experience Manager</li></ul> |

Pour plus d’informations sur la disponibilité des agents dans les applications Experience Cloud, consultez la [documentation d’Agentic AI dans Experience Cloud](https://experienceleague.adobe.com/fr/docs/core-services/interface/features/agentic-ai).

### Base de connaissances {#knowledge-base}

La base de connaissances fournit aux agents un accès sécurisé à l’intelligence commerciale des clients par le biais de sources de données structurées et non structurées, notamment la documentation du produit Adobe, les métadonnées du client sur les objets commerciaux et les données d’analyse.

## Accès {#access}

Les demandes de l’assistant AI sont authentifiées à l’aide des services Adobe Identity Management. Les autorisations sont appliquées par le contrôle d’accès Adobe Experience Platform et le contrôle d’accès Customer Journey Analytics.

Pour accéder à l’interface conversationnelle de l’assistant AI et utiliser un ou plusieurs agents Experience Platform, votre administrateur Adobe doit vous accorder les autorisations appropriées dans l’interface utilisateur des autorisations ou le Adobe Admin Console :

* **Real-Time CDP** et **Adobe Journey Optimizer** : votre administrateur doit vous accorder l’autorisation **Activer l’assistant AI** pour vous permettre d’accéder à l’assistant AI. Votre administrateur doit également vous accorder les autorisations **Afficher les informations opérationnelles** pour vous permettre de poser des questions relatives aux informations opérationnelles dans l’assistant AI. Les deux autorisations sont définies par l’administrateur dans l’interface utilisateur des autorisations.

* **Customer Journey Analytics** : votre administrateur doit vous accorder l’autorisation d’accéder à l’assistant AI par le biais du contrôle d’accès de [Customer Journey Analytics](https://experienceleague.adobe.com/fr/docs/analytics-platform/using/technotes/access-control). Cela vous permet de poser des questions sur la connaissance des produits et les informations sur les données.

>[!NOTE]
>
>Les questions d’informations opérationnelles ne sont pas disponibles pour Customer Journey Analytics. Par conséquent, aucune autorisation supplémentaire ne s’applique.

* **Adobe Experience Manager** : votre administrateur doit vous accorder l’autorisation d’accéder à l’assistant AI via [Adobe Admin Console](https://helpx.adobe.com/fr/enterprise/using/admin-console.html).

