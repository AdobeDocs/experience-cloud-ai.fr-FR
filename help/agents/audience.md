---
title: Agent Audience
description: Découvrez comment utiliser Audience Agent pour créer des audiences, afficher les modifications d’audience, détecter les audiences en double et afficher les informations sur l’audience.
source-git-commit: 4bb6da3fe1abee98446df62c94730274e0931493
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 2%

---


# Agent Audience

>[!AVAILABILITY]
>
>Audience Agent est disponible pour tous les clients qui ont accès à l’assistant AI. Toutefois, vous aurez besoin des autorisations suivantes pour utiliser pleinement les fonctionnalités d’Audience Agent.
>
>**Afficher les segments** : cette autorisation vous permet d’utiliser Audience Agent pour afficher des informations sur les audiences directement dans l’assistant AI.
>
>**Gérer les segments** : pour obtenir l’autorisation, vous pouvez utiliser Audience Agent afin de créer de nouvelles audiences directement dans l’assistant AI.

Audience Agent vous permet d’obtenir des informations sur les audiences, notamment la détection des modifications importantes de la taille de l’audience, la détection des audiences en double, l’exploration de votre inventaire des audiences et la récupération de la taille de vos audiences.

## Cas d’utilisation pris en charge

L’assistant Audience Agent within AI prend en charge les cas d’utilisation suivants :

- Rechercher la taille de l’audience et détecter les modifications importantes de cette dernière

   - Vous pouvez ainsi trouver des audiences qui ont soudainement augmenté ou diminué, ce qui vous permet de mieux analyser les changements potentiels du marché

- Détecter les audiences en double

   - Vous pouvez ainsi réduire les redondances avec les audiences que vous avez créées

- Rechercher des audiences en fonction d’attributs complets ou partiels nommés

   - Vous pouvez ainsi parcourir plus facilement votre inventaire d’audiences

- Découvrir les champs XDM que vous pouvez utiliser pour définir une audience

   - Cette compétence vous permet d’identifier plus facilement les champs à utiliser dans votre audience en fonction du contexte et de la pertinence

Audience Agent ne prend pas **actuellement** en charge les fonctionnalités suivantes :

- Création d’audiences basées sur les connaissances

   - La création d’une audience basée sur les connaissances consiste à créer une audience basée sur les attributs et les événements donnés
   - De plus, vous pouvez estimer la taille potentielle de l’audience avant la création de l’audience. Vous pouvez ainsi itérer rapidement sur l’audience la plus efficace avant qu’elle ne soit prête à être activée
   - La prise en charge de cette fonctionnalité sera bientôt disponible

- Exploration des audiences basée sur des objectifs

   - L’exploration des audiences basée sur des objectifs vous permet de découvrir des jeux de données et des profils pertinents alignés sur un objectif commercial en appliquant des modèles de machine learning tels que la propension à acheter ou à convertir.

En outre, lors de l’utilisation d’Audience Agent, vous devez tenir compte des contraintes suivantes :

- Audience Agent a besoin d’au moins 24 heures pour traiter vos données

   - Par exemple, vous **pouvez pas** une requête qui recherche des données au cours des dernières 24 heures. Vous devrez vérifier dans les 48 dernières heures, au minimum.

- Audience Agent ne prend en charge que les audiences basées sur les **personnes** qui sont évaluées à l’aide de la segmentation par lots

## Exemples d’invites

Les exemples suivants présentent des exemples d’invites et de réponses pour Audience Agent.

### Exploration des audiences de conversation

Afficher les champs pour les acheteurs aisés.

+++ Réponse

![L’assistant AI affiche un tableau présentant les champs pertinents pour les acheteurs aisés.](./images/audience/affluent-buyers.png)

+++

Quelles audiences n’ont été activées ou utilisées dans aucune campagne au cours des 30 derniers jours ?

+++ Réponse

![L’assistant AI affiche un tableau qui affiche les audiences qui n’ont pas été activées ou utilisées dans des campagnes au cours des 30 derniers jours.](./images/audience/not-activated.png)

+++

Répertoriez toutes les audiences qui ont été mappées à de nouvelles destinations au cours des 3 derniers mois.

+++ Réponse

![L’assistant AI répertorie l’audience qui a été mappée à une nouvelle destination au cours des 3 derniers mois.](./images/audience/new-destination.png)

+++

### Détecter les audiences en double

Existe-t-il des audiences avec des descriptions identiques ou similaires ?

+++ Réponse

![L’assistant AI affiche un tableau contenant la définition de segment et les noms des audiences avec les mêmes définitions de segment.](./images/audience/similar-descriptions.png)

+++

Identifiez les audiences qui ont les mêmes règles, mais des noms différents.

+++ Réponse

![L’assistant AI affiche un tableau contenant les noms des audiences qui partagent les mêmes règles d’audience.](./images/audience/same-rules-different-names.png)

+++

Montrez-moi toutes les audiences qui ont les mêmes règles, mais des destinations d’activation différentes.

+++ Réponse

![L’assistant AI indique qu’il n’existe aucune définition de segment en double vers différentes destinations.](./images/audience/same-rules-different-destinations.png)

+++

### Récupérer la taille de l’audience

Quelle est la taille actuelle de mon audience « Membres Gold-star en Californie_f153e1 » ?

+++ Réponse

![&#x200B; L’assistant d’IA indique la taille actuelle de l’audience qui a fait l’objet d’une question.](./images/audience/current-size.png)

+++

Quel est mon public le plus important ?

+++ Réponse

![L’assistant AI fournit des informations sur l’audience qui a le plus de profils, y compris le nom et l’ID d’audience.](./images/audience/largest-audience.png)

+++

### Détecter les modifications importantes de la taille de l’audience

Quelles audiences ont augmenté leur taille de plus de 20 % au cours de la dernière semaine ?

+++ Réponse

![&#x200B; L’assistant AI affiche un tableau qui répertorie les noms de toutes les audiences qui correspondent à la requête. Elle affiche également le pourcentage d’augmentation, la taille actuelle de l’audience, ainsi que la taille précédente de l’audience.](./images/audience/increase-past-week.png)

+++

Quelles audiences ont vu leur taille diminuer de plus de 10 % au cours du dernier mois ?

+++ Réponse

![&#x200B; L’assistant AI affiche un tableau qui répertorie les noms de toutes les audiences qui correspondent à la requête. Elle affiche également la taille de l’audience actuelle, la taille de l’ancienne audience, ainsi que la date de l’ancienne audience.](./images/audience/decrease-month.png)

+++

Quelle est mon audience qui croît le plus rapidement ?

+++ Réponse

![L’assistant d’IA indique le nom de l’audience qui croît le plus rapidement, ainsi que la taille actuelle et le pourcentage de croissance.](./images/audience/fastest-growing.png)

+++

## Étapes suivantes

Vous êtes arrivé au bout de ce guide, vous devriez mieux comprendre Audience Agent et les fonctionnalités qu’il prend en charge. Pour plus d’informations sur les agents dans Adobe Experience Platform, lisez la présentation d’[Agent Orchestrator](./agent-orchestrator.md).

