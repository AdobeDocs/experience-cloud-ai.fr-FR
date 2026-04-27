---
title: Journey Agent Overview and User Guide
description: Comprehensive guide to Journey Agent, enabling users to create, analyze, and optimize marketing journeys using a natural language interface in Journey Optimizer.
solution: Journey Optimizer
product: journey optimizer
role: Admin,User,Developer,Leader
TQID: https://experienceleague.adobe.com/7Bamc-q4rDOB9i0oxwixdmtdU8lrx3btpvMfAsjGnig
product_v2:
  - id: cb954087-f4fc-4456-afb9-e939cabcdc79
feature_v2:
  - id: baecb07f-ce89-4ebb-9cd9-0f7c053f944f
  - id: d0a62d3c-b79e-47e4-929e-40ef3cffa037
  - id: d556b755-390a-43f0-be32-a08cf6236126
  - id: d998adac-2f81-400b-a669-d07bb196e4eb
  - id: df64005d-8f9a-422e-ba4d-c6f6dc3454b4
  - id: fe338112-e2ce-4876-8989-fc4d497613f1
subfeature_v2:
  - id: b15c7c2e-788c-4eb7-86a8-390565b0d2c9
  - id: b32bb433-f8c6-4931-8e52-e657230a3bf2
  - id: b3a93754-a8b8-46eb-9421-7eccaeeb3dff
  - id: fa683eda-48de-4558-af32-2673edcd44fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: ff2b9b37-92e0-45fc-b853-379d44c08c89
source-git-commit: dd7883d8eccab3b0f006d55a850248e1c347d7e7
workflow-type: tm+mt
source-wordcount: 2655
ht-degree: 15%

---

# Journey Agent: Overview and User Guide

## Introduction to Journey Agent in Adobe Journey Optimizer

Journey Agent enables Journey Optimizer users to create, analyze, and optimize marketing journeys using a natural language interface. Avec l’agent Journey, les personnes professionnelles peuvent rapidement créer des parcours, détecter et résoudre les conflits de plannings ou d’audiences, analyser les performances et les points d’abandon, et identifier les parcours les plus performants à reproduire pour les campagnes futures. It empowers practitioners to make data-driven decisions, improve customer engagement, and streamline journey orchestration.

Journey Agent consists of three main jobs to be done:

- **Journey Create**: Build and configure marketing journeys through natural language prompts
- **Channel Content Create**: Generate, edit, and manage channel-specific content (email, push, SMS) for journeys using AI-powered content generation
- **Journey Analyze**: Analyze journeys, detect issues, uncover insights, and optimize customer engagement

## Journey Create: Use cases, Agentic skills and User guide

## Vue d’ensemble

Journey Create enables Journey Optimizer users to build and configure marketing journeys using a natural language interface. With Journey Create, practitioners can quickly create journeys by describing their requirements in conversational prompts. L’agent simplifie la création de parcours, ce qui permet aux spécialistes marketing de se concentrer sur la stratégie plutôt que sur la configuration technique.

>[!AVAILABILITY]
>
>Journey Create is available for all customers who have access to AI Assistant. However, you will need the following permissions in order to fully use Journey Create features:
>
>**Manage Journeys**: This permission lets you create new journeys directly in AI Assistant.
>
>**View Journey Events, Data Sources and Actions**: This permission ensures that the AI Assistant can search through Journey Events and Custom Actions.
>
>**View Segments**: This permission ensures that AI Assistant can search for audience segments when creating a Journey.
>
>**Manage Segments**: This permission lets you create new audiences directly in AI Assistant.

## Cas d’utilisation

### Key use cases for Journey Create

Journey Create offers capabilities that can be leveraged to accelerate marketing execution:

1. **Event-triggered journey creation**

   - Create journeys that activate based on specific customer events.
   - Design automated responses to customer actions in real-time.
   - Build personalized communication flows based on customer behavior.

1. **Audience-targeted journey creation**

   - Build journeys targeting specific audience segments.
   - Design multi-step communication sequences with strategic timing.

1. **Business-event triggered journey creation**

   - Create journeys that activate based on a particular business event and target a specified audience (e.g. product back in stock or game score change)
   - Build personalized communication flows based on customer behavior.

1. **Audience qualification journey creation**

   - Create journeys that activate as profiles enter or exit an audience segment definition.
   - Build personalized communication flows based on customer behavior.

1. **Conditional journey flows**

   - Create decision branches based on customer attributes.
   - Design split paths that adapt to customer preferences.

For each of these use cases, the agent translates natural language requirements into structured journey configurations.

## In scope and out of scope skills

### **In scope**

The following capabilities are supported by Journey Create:

- **Natural language journey creation**: Allows users to describe journey flow in conversational language.
- **Event-based and audience-based journeys**: Supports both trigger-based and scheduled journey types, also business event and audience qualification.
- **Conditional logic**: Handles decision splits and branching based on customer attributes.
- **Multi-channel messaging**: Supports push notifications, email, and SMS channels.
- **Journey scheduling**: Configures start dates and timing for scheduled journeys.

### **Out of scope**

Les fonctionnalités suivantes ne sont pas prises en charge actuellement :

- **Advanced journey analytics**
- **Real-time journey modifications**
- **Orchestration entre parcours**
- **Configuration des tests A/B**
- **Transformations de données complexes**

## Exemples d’invites

### Invites courantes pour la création de parcours

Voici des exemples d’invites utiles que les utilisateurs peuvent utiliser pour créer des parcours.

### Invites de parcours déclenchées par un événement

**parcours de visite de la boutique :**

« Créez un parcours qui démarre lorsqu’un utilisateur saisit l’emplacement de ma boutique. Envoyez une notification push pour souhaiter la bienvenue aux utilisateurs dans le magasin . Patientez 2 jours et vérifiez si l’utilisateur dispose d’une adresse e-mail valide. Si l’utilisateur dispose d’une adresse e-mail valide, envoyez une enquête par e-mail pour lui demander des informations sur son expérience en magasin. Si l’utilisateur ne dispose pas d’une adresse e-mail valide, envoyez une notification push pour demander l’enregistrement. »

**parcours après achat :**

« Créez un parcours qui démarre lorsqu’un client effectue un achat en ligne. Envoyez une notification push pour les remercier de leur achat. Ensuite, vérifiez s’il s’agit de membres du programme de fidélité. Si l’utilisateur est membre du programme de récompenses de fidélité, envoyez une seconde notification push avec un code de remise de 10 %. Si l’utilisateur n’est pas membre du programme de récompenses de fidélité, envoyez une notification push l’invitant à s’inscrire au programme de fidélité. Patientez 2 jours et envoyez une notification push de suivi avec une enquête sur leur expérience d’achat. »

**Promotion basée sur un événement :**

« Créez un parcours déclenché lorsque le score du jeu atteint 50. Envoyez un SMS aux membres de la récompense de fidélité pour les informer qu’ils sont éligibles à une part gratuite de pizza du sponsor partenaire. »

### Invites de parcours ciblé sur l’audience

**Campagne saisonnière :**

« Je veux créer un parcours ciblant un public de randonneurs d&#39;un jour. Je souhaite envoyer un e-mail pour avertir cette audience de ma prochaine vente de vacances qui comprend divers articles essentiels pour la randonnée. Patientez 3 jours après l’envoi du premier e-mail et envoyez un second e-mail contenant un coupon de 15 % avec une livraison gratuite. Patientez 1 semaine, puis envoyez un 3e e e e-mail pour montrer notre nouveau sac de couchage et notre nouvelle collection de tente. Planifiez le parcours pour qu’il démarre le 20/12. »

**Appréciation de la fidélité :**

« Créez un parcours de reconnaissance de la fidélité pour les propriétaires de SUV, y compris une notification push de remerciement avec une offre de lavage de voiture gratuite et un rappel de notification push de suivi si la première notification n’est pas interactive dans un délai d’un jour. »

### Invites ouvertes

Pour les utilisateurs et utilisatrices commençant sans avoir à l’esprit un parcours spécifique :

- « Je voudrais créer un parcours »
- « Aide-moi à créer un parcours »
- « Création d&#39;un parcours »

L’agent vous fournira des conseils et des exemples pour vous aider à définir vos exigences en matière de parcours.

## Bonnes pratiques

### Bonnes pratiques en matière de promotion

Pour optimiser l’efficacité de Parcours Create, appliquez les bonnes pratiques suivantes :

1. **Soyez précis** : donnez des détails clairs sur vos objectifs de parcours, votre audience cible et les actions souhaitées. Incluez des informations sur les canaux, la durée et les conditions.
1. **Spécifier le minutage** : indiquez clairement les périodes d’attente entre les actions et le moment où le parcours doit démarrer.
1. **Définir des conditions** : lors de l’utilisation d’une logique conditionnelle, expliquez les critères de chaque chemin de branche.
1. **Inclure les canaux** : indiquez les canaux de communication à utiliser (push, e-mail, SMS).
1. **Mentionner la planification** : pour les parcours planifiés, indiquez la date et l’heure de début souhaitées.
1. **Actions personnalisées** : si vous utilisez des actions personnalisées dans votre workflow, vous devez indiquer que vous utilisez une action personnalisée avec le nom exact de l’action personnalisée. Exemple :
Lorsqu’un utilisateur accède à l’emplacement de ma boutique, envoyez un message de bienvenue à l’aide d’une action personnalisée ExternalPush. Patientez 2 jours, puis envoyez un message de relance à l’aide d’une action personnalisée ExternalEmail avec un questionnaire lors de leur visite.
1. **Valider les expressions** : veillez à vérifier et à valider toutes les expressions créées par Journey Agent pour vous assurer que les champs et valeurs corrects sont utilisés.

### Bonnes pratiques de configuration

- **Définir des objectifs clairs** : avant de créer des parcours, établissez des objectifs clairs (amélioration de la rétention, stimulation des conversions, augmentation de l’engagement).
- **Préparer les audiences** : assurez-vous que les audiences cibles sont déjà créées et correctement segmentées.
- **Planifier le contenu du message** : définissez votre stratégie de messagerie avant la création du parcours.
- **Tenir compte de l’expérience client** : concevez des flux de parcours qui respectent les préférences des clients et évitent la surcommunication.

## Création de contenu de canal : cas d’utilisation, compétences techniques et guide de l’utilisateur

>[!AVAILABILITY]
>
>Cette fonctionnalité est disponible pour tous les clients en disponibilité limitée. Contactez votre représentant ou représentante Adobe pour en obtenir l’accès.

## Vue d’ensemble

La création de contenu de canal permet aux utilisateurs de Journey Optimizer de générer, modifier et gérer du contenu spécifique au canal pour les parcours à l’aide de la génération de contenu optimisée par l’IA.

## Cas d’utilisation

### Cas d’utilisation clés de la création de contenu de canal

1. **Génération de contenu spécifique à un canal** : générez du contenu pour les e-mails, les notifications push, les SMS et d’autres canaux à l’aide d’invites en langage naturel.

1. **Création de contenu basé sur des modèles** : recherchez et sélectionnez des modèles disponibles avec des fonctionnalités d’aperçu.

1. **Gestion de contenu multicanal** : générez et gérez du contenu pour plusieurs canaux au sein du même workflow de parcours.

1. **Modification de contenu en contexte** : ouvrez le contenu généré dans Content Designer pour le modifier et l’affiner.

1. **Affinement et itération du contenu** : générez à nouveau du contenu avec des tons ou des styles différents à l’aide de l’action Régénérer.

1. Intégration de la zone de travail de Parcours **&#x200B;**&#x200B;: sélectionnez les parcours dans l’inventaire et affichez les canaux associés.

## Compétences incluses et exclues

### **Dans la portée**

Les fonctionnalités suivantes sont prises en charge par la création de contenu de canal :

- **Génération de contenu optimisée par l’IA** : générez du contenu pour les e-mails, les notifications push, les SMS et d’autres canaux à l’aide d’invites en langage naturel.
- **Gestion des modèles** : recherchez et sélectionnez un modèle disponible avec les fonctionnalités d’aperçu.
- **Modification en contexte** : ouvrez le contenu généré dans Content Designer pour le modifier et l’affiner.
- **Régénération du contenu** : générez à nouveau du contenu avec des tons, des styles ou des messages différents à l’aide de l’action Régénérer.
- **Prise en charge multicanal** : générez et gérez du contenu pour plusieurs canaux au sein du même workflow de parcours.
- **Accès à l’inventaire des Parcours** : sélectionnez les parcours dans l’inventaire et affichez les canaux associés.

### **Hors portée**

Les fonctionnalités suivantes ne sont pas prises en charge actuellement :

- **Alignement des marques et contrôles de la qualité du contenu**
- **Insérer des nœuds de contenu directement dans la zone de travail du parcours**
- **Importation de modèles**

## Exemples d’invites

### Génération de contenu

« Générer le contenu de l’e-mail pour mon parcours de bienvenue. Créez un e-mail de bienvenue pour les nouveaux clients avec un ton convivial et incluez une offre de remise de 10 %. »

« Ajouter du contenu pour l’e-mail du canal pour mon parcours de bienvenue. »

« Générer une notification push pour le parcours de visite de ma boutique. Créez un message de bienvenue qui encourage les clients à s’enregistrer et à recevoir une offre spéciale. »

« Générer du contenu SMS pour mon parcours déclenché par un événement. Créez un court message informant les clients d’une vente flash avec un call-to-action. »

### Sélection de modèles

« Montrez-moi les modèles d’e-mail disponibles pour mon parcours de campagne saisonnier. »

« Sélectionnez un modèle d’e-mail au design moderne et épuré. »

### Modification et affinement du contenu

« Ouvrez le contenu de l’e-mail dans le Designer de contenu afin que je puisse personnaliser la conception. »

« Régénérez le contenu de la notification push avec un ton plus décontracté. »

« Mettez à jour le contenu de l’e-mail pour inclure un code promotionnel. »

## Bonnes pratiques

### Bonnes pratiques en matière de promotion

1. **Soyez précis** : fournissez des détails clairs sur le type de contenu, le ton, l’audience cible et les messages clés.
1. **Spécifier le canal** : indiquez clairement pour quel canal vous créez du contenu (e-mail, notification push, SMS).
1. **Définir le ton** : spécifiez le ton souhaité (amical, formel, informel, urgent).
1. **Itérer et affiner** : utilisez l’action de régénération pour affiner le contenu jusqu’à ce qu’il réponde à vos besoins.

## Analyse de parcours : cas d’utilisation, compétences agences et guide de l’utilisateur

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

### Cas d’utilisation clés de l’analyse de Parcours

L’analyse de parcours offre un éventail de fonctionnalités qui peuvent être exploitées pour optimiser les efforts marketing :

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

Parcours Analyze prend en charge les fonctionnalités suivantes :

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

- « Combien de parcours actifs ai-je ? »
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

Pour optimiser l’efficacité de l’analyse de Parcours, appliquez les bonnes pratiques suivantes :

1. **Être précis** : utilisez des questions claires et concises pour obtenir des informations ciblées. Par exemple, au lieu de demander « Quels sont mes parcours ? », indiquez « Répertorier tous les parcours créés le mois dernier ».
1. **Combiner les informations** : intégrez les informations de l’agent Audience et de l’agent Data Insights pour obtenir une vue d’ensemble des performances des parcours.
1. **Affinage itératif** : utilisez l’analyse des abandons et des chevauchements pour affiner de manière itérative la conception et le planning des parcours.

### Bonnes pratiques de configuration

- **Définir des objectifs clairs** : avant d’analyser les parcours, définissez des objectifs clairs (par exemple, améliorer la fidélisation, augmenter les conversions).
- **Contrôler régulièrement** : planifiez des vérifications régulières des performances des parcours afin d’identifier les tendances et les anomalies.
- **Optimiser la segmentation** : veillez à ce que la segmentation de l’audience soit équilibrée afin d’éviter la lassitude et de maximiser l’engagement.

## Diapositives et présentations

>[!NOTE]
>
>Des diapositives et des documents de présentation pour Journey Agent seront disponibles ici. Consultez bientôt les mises à jour.
