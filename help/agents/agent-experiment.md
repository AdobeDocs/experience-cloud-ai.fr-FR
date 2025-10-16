---
title: Agent d’expérimentation
description: Découvrez comment utiliser l’agent d’expérience
source-git-commit: 0069a97bcb35f609019ec32f263175a36525161a
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 3%

---

# Agent d’expérimentation

>[!AVAILABILITY]
>
>L’agent d’expérimentation est disponible pour tous les clients qui ont accès à l’assistant AI. Cependant, vous avez besoin des autorisations suivantes pour utiliser pleinement les fonctionnalités de l’agent d’expérience.
>
>**Afficher les expériences** : cette autorisation vous permet d’utiliser l’agent d’expérimentation pour afficher des informations sur l’expérience directement dans l’assistant AI.
>
>**Gérer les métadonnées d’expérience** : cette autorisation vous permet d’utiliser l’agent d’expérience pour créer de nouvelles expériences directement dans l’assistant AI.

## Vue d’ensemble

Le **agent d’expérimentation** est un outil optimisé par l’IA qui modernise la manière dont vous pouvez exécuter et gérer des expériences numériques sur des sites web, des e-mails, des messages push et des applications. Basé sur la plateforme d’IA et les outils d’expérimentation de Adobe Experience Platform, le **Agent d’expérimentation** vous permet d’exécuter des expériences plus efficacement, d’organiser les objectifs commerciaux et de générer des informations exploitables, en mettant en évidence ce qui a fonctionné, ce qui n’a pas fonctionné et où tester ensuite.

Dans le cadre de la fonctionnalité Experimentation Accelerator, l’agent fournit :

* **Performances** : une vue claire de ce qui s’est passé dans l’expérience.

* **Insights** : explication des raisons pour lesquelles les résultats se sont produits

* **Opportunités** : conseils sur les prochaines actions à entreprendre

![Exemple pour l’agent d’expérience](./images/experiment/experiment-agent.png)

## Cas d’utilisation

L’agent d’expérimentation améliore chaque phase du workflow d’expérimentation en analysant les résultats, en interprétant le contenu et en suggérant les étapes suivantes.

Ses fonctionnalités peuvent être regroupées en cinq fonctions clés :

* **Résumé des expériences**

  Fournir aux parties prenantes un aperçu clair et non technique des résultats des expériences.

* **Analyse de contenu**

  Examinez les messages ou les éléments créatifs des traitements pour comprendre pourquoi certains ont surpassé les autres.

* **Identification des attributs**

  Classez les traitements en fonction de leurs attributs clés, par exemple, thèmes, tons, formats, et connectez ces attributs aux résultats de conversion.

* **génération de recommandations**

  Suggérez de nouveaux traitements ou ajustements à tester, en fonction des informations issues d’expériences précédentes.

* **Opportunités**

  Identifiez des zones plus larges ou de nouveaux angles d’expérimentation pour découvrir le potentiel inexploité.

## Fonctionnalités In Scope et Out of Scope

### **Dans le champ d’application**

Les fonctionnalités suivantes sont actuellement prises en charge :

* Performances
* Insights
* Opportunités

### **Hors du champ d’application**

Les fonctionnalités suivantes ne sont pas prises en charge actuellement :

* Création ou modification d’expériences
* Utilisation de plusieurs mesures pour la création de rapports sur les cas d’utilisation

## Exemples d’invites

Voici une liste d’exemples d’invite pour vous aider à prendre en main l’agent d’expérimentation :

### Questions générales

| Invites |
|-|
| Quelles sont les expériences en cours d’exécution ? |
| Quelles expériences sont en cours d’exécution pour le `<campaign name>` ? |
| Quelles expériences ont commencé le mois dernier ? |
| Combien d’expériences se sont terminées l’année dernière ? |
| Quelles expériences sont actuellement en pause/arrêtées/etc ? |
| Quels schémas communs émergent des tests récents ? |
| Quelle est la durée moyenne des expériences au cours du dernier trimestre ? |

### Questions relatives aux performances

| Invites |
|-|
| Pour ma `<experiment name>`, quel traitement mène-t-on? |
| Quel est l&#39;ascenseur du `<experiment name>` ? |
| Quelles expériences ont donné des résultats statistiquement significatifs ? |
| Quelles expériences ont eu le meilleur taux de conversion ? |

### Questions sur Insights

| Invites |
|-|
| Qu’est-ce que le test `<experiment name>` ? |
| Qu&#39;avons-nous appris de l&#39;`<experiment name>` ? |
| Pouvez-vous me dire pourquoi le traitement A a gagné ? |
| Quels sont les thèmes les plus populaires dans les variantes gagnantes ? |
| Quels schémas communs émergent des tests récents ? |
| Est-ce que quelque chose d&#39;inattendu s&#39;est produit en `<experiment name>` ? |

### Questions relatives aux opportunités

| Invites |
|-|
| Que me recommandez-vous de faire ensuite après cette expérience ? |
| Y a-t-il un moyen d&#39;améliorer la `<experiment name>` ? |
| Quelles opportunités sont devenues plus claires après `<experiment name>` ? |
| Que puis-je tester ensuite pour prouver l’hypothèse de `<experiment name>` ? |
| Quels cas d’utilisation supplémentaires dois-je implémenter ? |
