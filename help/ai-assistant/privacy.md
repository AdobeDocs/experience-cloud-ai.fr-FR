---
title: Assistant Confidentialité, sécurité et gouvernance dans l’IA
description: Découvrez les pratiques en matière de confidentialité, de sécurité et de gouvernance pour l’assistant AI.
source-git-commit: fe4d2de03e34eccd2950f87b3c57ffbb5e1cf5e9
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Assistant Confidentialité, sécurité et gouvernance dans l’IA

L’assistant AI de Adobe Experience Platform place la confidentialité, la sécurité et la gouvernance au premier plan.

Lisez ce document pour en savoir plus sur les fonctionnalités axées sur la confiance du client que vous pouvez attendre de l’assistant AI :

* Aucune donnée personnelle n&#39;est actuellement utilisée par AI Assistant, même à des fins de formation.
* L’assistant AI ne connaît pas les données des consommateurs.
* Toutes les politiques [de contrôle d’accès](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home) existantes seront respectées par l’assistant AI.

   * Toutes les nouvelles politiques de contrôle d’accès basé sur les attributs sont reflétées dans l’assistant AI après un maximum de 24 heures&amp;ast;

* Vous devez disposer d’autorisations explicites pour interagir avec l’assistant AI.

   * Vous pouvez définir différemment les autorisations pour Experience Platform et Journey Optimizer à l’aide de l’interface utilisateur [Autorisations](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/permissions-ui/browse) et utiliser [Admin Console](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/ui/browse) pour attribuer des autorisations à Customer Journey Analytics.
   * Les autorisations sont granulaires et l’administrateur de votre sandbox peut configurer quelles catégories de questions peuvent être posées par vos utilisateurs (questions basées sur les connaissances du produit avec l’assistant AI ou questions sur les informations opérationnelles).

* L’assistant AI est une fonctionnalité conforme à la loi HIPAA lorsqu’il est utilisé en combinaison avec Adobe Experience Platform Healthcare Shield.
* Vous pouvez consulter un journal de vos interactions précédentes avec l’assistant AI avec une politique de conservation de 30 jours.
* L’assistant AI repose sur des données spécifiques aux sandbox et sur la documentation publique d’Adobe lorsqu’il répond aux invites des utilisateurs. Les données ne sont pas partagées entre les sandbox.
* Les invites que vous fournissez à l&#39;assistant AI ne sont pas partagées avec les autres clients.

&amp;ast; *Cela implique que si de nouveaux libellés sont ajoutés aux champs et aux objets ou si de nouvelles politiques sont créées, l’assistant AI mettra jusqu’à 24 heures pour les honorer. Pendant ces 24 heures, les utilisateurs disposant d’un accès nouvellement restreint peuvent toujours accéder à ces champs et objets.*
