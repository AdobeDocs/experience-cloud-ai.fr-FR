---
title: Présentation de Journey Agent et guide de l’utilisateur
description: Guide complet de Journey Agent permettant aux utilisateurs de créer, d’analyser et d’optimiser des parcours marketing à l’aide d’une interface en langage naturel dans Journey Optimizer.
solution: Journey Optimizer
product: journey optimizer
role: Admin,User,Developer,Leader
source-git-commit: 0e3839f829efc5670c235435d49ed5e49da2ed13
workflow-type: tm+mt
source-wordcount: '2147'
ht-degree: 18%

---


# Journey Agent : présentation et guide de l’utilisateur

## Présentation de Journey Agent dans Adobe Journey Optimizer

Journey Agent permet aux utilisateurs de Journey Optimizer de créer, d’analyser et d’optimiser des parcours marketing à l’aide d’une interface en langage naturel. Avec l’agent Journey, les personnes professionnelles peuvent rapidement créer des parcours, détecter et résoudre les conflits de plannings ou d’audiences, analyser les performances et les points d’abandon, et identifier les parcours les plus performants à reproduire pour les campagnes futures. Il permet aux professionnels de prendre des décisions basées sur les données, d’améliorer l’engagement des clients et de rationaliser l’orchestration des parcours.

Journey Agent se compose de deux compétences principales :
- **Parcours Create Agent** : crée et configure des parcours marketing à l’aide d’invites en langage naturel
- **Agent d’analyse de Parcours** : analysez les parcours, détectez les problèmes, découvrez des informations et optimisez l’engagement des clients

&#x200B;---

&#x200B;# Parcours Create Agent : présentation des compétences et guide de l’utilisateur

## Vue d’ensemble

L’agent de création de parcours permet aux utilisateurs de Journey Optimizer de créer et de configurer des parcours marketing à l’aide d’une interface en langage naturel. Avec l’agent de création de Parcours, les utilisateurs et utilisatrices peuvent rapidement créer des parcours en décrivant leurs besoins dans des invites conversationnelles. L’agent simplifie la création de parcours, ce qui permet aux spécialistes du marketing de se concentrer sur la stratégie plutôt que sur la configuration technique.

>[!AVAILABILITY]
>
>Le Parcours Créer un agent est disponible pour tous les clients qui ont accès à l’assistant AI. Toutefois, vous aurez besoin des autorisations suivantes pour utiliser pleinement les fonctionnalités de création d’agent de Parcours :
>
>**Gérer les Parcours** : cette autorisation vous permet de créer des parcours directement dans l’assistant AI.
>
>**Afficher les événements de Parcours, les sources de données et les actions** : cette autorisation permet à l’assistant AI de rechercher des événements de Parcours et des actions personnalisées.
>
>**Afficher les segments** : cette autorisation permet à l’assistant AI de rechercher des segments d’audience lors de la création d’un Parcours.
>
>**Gérer les segments** : cette autorisation vous permet de créer de nouvelles audiences directement dans l’assistant AI.

## Cas d’utilisation

### Cas d’utilisation clés de l’agent de création de Parcours

La compétence Parcours Créer un agent offre des fonctionnalités qui peuvent être exploitées pour accélérer l’exécution marketing :

1. **Création de parcours déclenchée par un événement**

   - Créez des parcours qui s’activent en fonction d’événements client spécifiques.
   - Concevez des réponses automatisées aux actions des clients en temps réel.
   - Créez des flux de communication personnalisés en fonction du comportement des clients.

1. **Création de parcours ciblés sur l’audience**

   - Créez des parcours ciblant des segments ciblés spécifiques.
   - Concevez des séquences de communication à plusieurs étapes avec un timing stratégique.

1. **Création de parcours déclenchée par un événement métier**

   - Créez des parcours qui s’activent en fonction d’un événement métier particulier et ciblent une audience spécifiée (par exemple, retour du produit en stock ou changement du score du jeu).
   - Créez des flux de communication personnalisés en fonction du comportement des clients.

1. **Création du parcours de qualification d’audience**

   - Créez des parcours qui s’activent lorsque les profils entrent ou sortent d’une définition de segment ciblé.
   - Créez des flux de communication personnalisés en fonction du comportement des clients.

1. **Flux de parcours conditionnels**

   - Créez des branches de décision en fonction des attributs du client.
   - Concevez des chemins de division qui s’adaptent aux préférences des clients.

Pour chacun de ces cas d’utilisation, l’agent traduit les exigences en langage naturel en configurations de parcours structurées.

## Compétences incluses et exclues

### **Dans la portée**

Les fonctionnalités suivantes sont prises en charge par l’agent de création de Parcours :

- **Création de parcours en langage naturel** : permet aux utilisateurs de décrire le flux du parcours dans un langage de conversation.
- **parcours basés sur un événement et sur une audience** : prend en charge les types de parcours planifiés et basés sur un déclencheur, ainsi que la qualification des événements métier et des audiences.
- **Logique conditionnelle** : gère les divisions de décision et l’embranchement en fonction des attributs du client.
- **Messagerie multicanal** : prend en charge les canaux de notification push, d’e-mail et de SMS.
- **Planification des Parcours** : configure les dates et heures de début des parcours planifiés.

### **Hors portée**

Les fonctionnalités suivantes ne sont pas prises en charge actuellement :

- **Analyses de parcours avancées**
- **Modifications du parcours en temps réel**
- **Orchestration entre parcours**
- **Configuration des tests A/B**
- **Transformations de données complexes**
- **Création du message de contenu**

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

Pour optimiser l’efficacité de l’action Créer un agent de Parcours, suivez les bonnes pratiques suivantes :

1. **Soyez précis** : donnez des détails clairs sur vos objectifs de parcours, votre audience cible et les actions souhaitées. Incluez des informations sur les canaux, la durée et les conditions.
1. **Spécifier le minutage** : indiquez clairement les périodes d’attente entre les actions et le moment où le parcours doit démarrer.
1. **Définir des conditions** : lors de l’utilisation d’une logique conditionnelle, expliquez les critères de chaque chemin de branche.
1. **Inclure les canaux** : indiquez les canaux de communication à utiliser (push, e-mail, SMS).
1. **Mentionner la planification** : pour les parcours planifiés, indiquez la date et l’heure de début souhaitées.
1. **Actions personnalisées** : si vous utilisez des actions personnalisées dans votre workflow, vous devez indiquer que vous utilisez une action personnalisée avec le nom exact de l’action personnalisée. Exemple :
Lorsqu’un utilisateur accède à l’emplacement de ma boutique, envoyez un message de bienvenue à l’aide d’une action personnalisée ExternalPush. Patientez 2 jours, puis envoyez un message de relance à l’aide d’une action personnalisée ExternalEmail avec un questionnaire lors de leur visite.
1. **Valider les expressions** : veillez à vérifier et à valider toutes les expressions créées par Journey Agent pour vous assurer que les champs et valeurs corrects sont utilisés.

### Bonnes pratiques de configuration

- **Définir des objectifs clairs** : avant de créer des parcours, établissez des objectifs clairs (amélioration de la rétention, stimulation des conversions, augmentation de l’engagement).
- **Préparer les audiences** : assurez-vous que les audiences cibles sont déjà créées et correctement segmentées.
- **Planifier le contenu du message** : définissez votre stratégie de messagerie avant la création du parcours.
- **Tenir compte de l’expérience client** : concevez des flux de parcours qui respectent les préférences des clients et évitent la surcommunication.

&#x200B;---

&#x200B;# Agent Parcours Analyze : présentation des compétences et guide de l’utilisateur

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

&#x200B;---

## Diapositives et présentations

>[!NOTE]
>
>Des diapositives et des documents de présentation pour Journey Agent seront disponibles ici. Consultez bientôt les mises à jour.
