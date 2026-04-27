---
title: IA dans les applications Experience Cloud
description: Découvrez comment les applications Experience Cloud utilisent l’IA générative (GenAI), l’Assistant IA et l’IA agentique.
TQID: https://experienceleague.adobe.com/heALjEZbowNaygG24oOM2HSlHa9oYVI5ViUNZDr19Ds
product_v2: id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: d095671a-1355-40aa-8b5f-06c33c68080bid: e1e0219c-f879-479f-8427-888ed2a6e9c2id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: dd7883d8eccab3b0f006d55a850248e1c347d7e7
workflow-type: tm+mt
source-wordcount: 846
ht-degree: 17%

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

[Adobe Experience Platform Agent Orchestrator](./agents/agent-orchestrator.md) est la nouvelle couche agentic de Adobe Experience Platform. Conçu pour exploiter la richesse des données et des connaissances clientèle de la plateforme, Experience Platform Agent Orchestrator alimente l’intelligence et le raisonnement d’agents experts spécialement conçus pour Adobe Experience Platform, leur permettant d’exécuter des prises de décision complexes et de résoudre des problèmes à grande vitesse et à grande échelle, le tout sous supervision humaine. Lorsque vous posez des questions ou demandez de l’aide en langage naturel dans une interface conversationnelle telle que l’assistant IA, Agent Orchestrator fait automatiquement appel à des agentes et agents spécialisés pour vous fournir les bonnes réponses. Agent Orchestrator se souvient de l’historique de vos conversations, ce qui lui permet de s’appuyer naturellement sur vos questions précédentes sans répéter le contexte et de combiner les informations issues de plusieurs agentes et agents afin de vous présenter des réponses claires et unifiées.

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

Available in Customer Journey Analytics, the Data Insights Agent:

- Answers questions about your data using natural language.
- Builds relevant visualizations in Analysis Workspace.
- Uses components from your dataview and actual data.

#### Agent d’analyse de parcours

The Journey Analyze Agent enables the Adobe Journey Optimizer users to:

- Analyze, and optimize journeys using natural language.
- Detect and resolve schedule or audience conflicts.
- Analyze performance and drop-off points.

Read the [Journey Agent documentation](./agents/ajo-agent.md) for more information.

#### Agent du support technique du produit

Use the Product Support Agent for self-serve debugging and troubleshooting:

- Troubleshoot Adobe Experience Platform features without leaving workflows.
- Create support tickets with context from AI Assistant interactions.
- Check ticket updates through AI Assistant.

Read the [Product Support Agent documentation](./agents/product-support.md) for more information.

<!--
#### Adobe Marketing Agent for [!DNL Microsoft 365 Copilot]

Use the Adobe Marketing Agent for [!DNL Microsoft 365 Copilot] to retrieve marketing insights from Experience Platform in [!DNL Microsoft 365] apps like [!DNL Teams], [!DNL Word], [!DNL Powerpoint], and [!DNL Excel]. With this agent, you can:

- Make faster, data-driven marketing decisions.
- Reduce time spent switching between tools.
- Simplify access to audience and journey insights across teams.

Read the [Adobe Marketing Agent documentation](./agents/ama-ms.md) for more information.
-->

## Prise en main

### Access requirements

To use AI Assistant and Experience Platform Agents, your Adobe Admin needs to set up the appropriate permissions:

- To use AI Assistant within Real-Time CDP and Adobe Journey Optimizer, you need the &quot;Enable AI Assistant&quot; permission, as well as the &quot;View Operational Insights&quot; permission to access operational questions.
- Access to AI Assistant in Customer Journey Analytics is managed through Customer Journey Analytics Access Control, which allows you to ask both product knowledge and data insights questions.
- For Adobe Experience Manager, you can access AI Assistant through permissions set in the Adobe Admin Console.

### Confidentialité et sécurité

AI Assistant is built with privacy, security, and governance at the forefront:

- No personal data is used for training.
- All existing access control policies are honored.
- HIPAA-ready when used with Adobe Experience Platform Healthcare Shield.
- 30-day retention policy for interaction logs.
- Sandbox-specific data isolation.

## Bonnes pratiques

Pour tirer le meilleur parti de votre expérience d’assistant d’IA, suivez ces bonnes pratiques :

- **Soyez précis** dans vos invites pour obtenir des informations ciblées et pertinentes de la part de l&#39;assistant d&#39;IA.
- **Vérifiez les réponses** en examinant les citations de la source et les explications de raisonnement fournies par l’assistant d’IA.
- **Utilisez le paramètre contextuel** pour vous assurer que les sources de données les plus pertinentes sont utilisées pour vos questions.
- **Faites des commentaires** pour améliorer les performances et la précision de l’assistant d’IA au fil du temps.
- **Combinez les informations** de plusieurs agents pour obtenir une analyse plus complète et mieux équilibrée.

## Considérations juridiques

Lors de l’utilisation de l’assistant d’IA, il est important de tenir compte des principales considérations juridiques et pratiques. Actuellement, l’assistant AI prend uniquement en charge les réponses en anglais. Veillez toujours à vérifier les informations fournies, car les modèles linguistiques peuvent parfois faire des erreurs. Utilisez les étapes de raisonnement et les explications incluses dans les réponses pour mieux comprendre les réponses que vous recevez. Si vous rencontrez des problèmes ou des inexactitudes, envoyez des commentaires pour améliorer l’assistant d’IA au fil du temps.
