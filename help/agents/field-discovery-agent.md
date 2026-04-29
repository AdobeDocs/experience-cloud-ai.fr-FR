---
title: Agent de découverte de champ
description: Recherchez, évaluez et sélectionnez des champs XDM dans Adobe Experience Platform à l’aide du langage naturel dans l’assistant AI, avec des résultats classés, des valeurs d’exemple et un contexte d’utilisation pour la segmentation, les requêtes et les workflows de données.
keywords: découverte de champs, XDM, assistant AI, agents Experience Platform, liaison d’entités, recommandations de champs, création d’audiences, segmentation
solution: Experience Platform
role: User, Admin, Developer
source-git-commit: b4d8c83cca73a19e1fe229c8cec03caee16bcd8c
workflow-type: tm+mt
source-wordcount: '3600'
ht-degree: 1%

---

# Agent de découverte de champ

Lors de la création d’audiences ou de l’intégration de données dans Adobe Experience Platform, l’identification du champ XDM approprié à un concept d’entreprise nécessite souvent une navigation manuelle dans les schémas ou une connaissance à l’avance du nom exact d’un champ. Différents champs peuvent représenter le même concept sous des noms différents (par exemple, état, région et emplacement) et le choix d’un champ incorrect introduit des erreurs dans les workflows en aval.

L’agent de découverte de champs est un agent optimisé par l’IA dans Adobe Experience Platform qui vous aide à rechercher, évaluer et sélectionner des champs XDM à l’aide de requêtes en langage naturel dans l’assistant IA. Vous décrivez ce que vous recherchez en langage clair (un concept d’entreprise, un objectif de workflow ou un nom de champ spécifique) et l’agent renvoie des suggestions de champs avec classement et contexte connexe.

L’agent de découverte de champ est appelé automatiquement en arrière-plan dans l’assistant AI lorsque d’autres agents Experience Platform doivent résoudre les références de champ ou d’entité. Dans ce cas, il fonctionne en arrière-plan pour améliorer la précision de l’agent avec lequel vous travaillez. Lorsque vous avez besoin de la découverte de champs pour votre propre travail, écrivez une invite explicite de recherche de champs dans l’assistant AI. L&#39;agent de découverte de champ affiche uniquement les informations de champ. Il ne modifie pas les schémas, les jeux de données ou les audiences et respecte vos contrôles d’accès existants et le contexte du sandbox.

## Quand l’utiliser {#when-to-use-this}

Utilisez l’agent de découverte de champ explicitement dans l’assistant AI lorsque vous avez besoin de suggestions de champs de classement, de valeurs d’exemple et de contexte d’utilisation pour un mappage, une segmentation ou une requête. Il est utilisé implicitement lorsqu’un autre agent Experience Platform l’appelle en arrière-plan pour résoudre les références de champ ou d’entité. Dans ce cas, vous restez dans le workflow de cet agent et n’envoyez pas d’invite de recherche de champ distincte.

## Conditions préalables {#prerequisites}

Pour utiliser l&#39;agent de détection de champ, vérifiez que vous disposez des éléments suivants :

- Accès à Adobe Experience Platform et à l’assistant AI
- L’organisation et le sandbox appropriés
- Accès aux schémas et aux jeux de données sur lesquels vous avez l’intention d’effectuer des requêtes

Une connaissance de base des schémas XDM et de l’utilisation des champs dans la segmentation ou les workflows de données peut vous aider à interpréter les résultats plus efficacement. Pour plus d’informations, consultez la [présentation de XDM](https://experienceleague.adobe.com/fr/docs/experience-platform/xdm/home) et la [documentation de l’éditeur de schémas](https://experienceleague.adobe.com/en/docs/experience-platform/xdm/tutorials/create-schema-ui).

Pour obtenir des instructions sur l’activation de l’accès de l’assistant AI et l’octroi des autorisations requises, consultez le [guide d’accès ](./agent-orchestrator.md#access).

## Fonctions de l’agent de découverte de champ {#field-discovery-agent-functions}

L&#39;agent de découverte de champ traite votre requête et renvoie l&#39;un des trois types de sortie selon votre intention. Ces fonctions reflètent la manière dont l’agent interprète votre requête ; vous ne les sélectionnez pas. L’agent détermine automatiquement le type de réponse approprié en fonction de ce que vous décrivez.

| Fonction | Description | Sortie attendue |
| --- | --- | --- |
| **Identification** | Identifie les champs XDM qui correspondent sémantiquement à un concept ou à un attribut métier que vous décrivez en langage naturel. | Une liste classée des champs candidats avec des libellés de pertinence, des chemins de champ et des liens vers des contextes d’utilisation. |
| **Recommandation** | Recommande des champs XDM en fonction d’un objectif de workflow ou d’un cas d’utilisation que vous décrivez, comme la création d’un segment d’audience ou la modélisation d’un attribut comportemental. | Liste hiérarchisée des champs pertinents par rapport à l’objectif déclaré, avec contexte de pertinence pour chacun. |
| **Enrichissement** | Renvoie le contexte détaillé d’un champ spécifique, y compris les exemples de valeurs, l’emplacement du schéma et l’endroit où le champ est utilisé dans les jeux de données, les audiences et les destinations. | Détails du champ dont les exemples de valeurs, le chemin du schéma, les jeux de données associés et l’utilisation de l’audience ou de la destination. |

## Fonctionnement de Field Discovery Agent {#how-field-discovery-agent-works}

À un niveau élevé, l’agent interprète votre intention, recherche vos données disponibles et classe les résultats par pertinence. La manière dont vous formulez votre requête affecte directement chaque étape, ce qui a un impact sur la qualité des résultats.

Lorsque vous envoyez une requête dans l’assistant AI, l’agent de découverte de champ traite la requête en trois étapes :

| Étape | Description |
|------|-------------|
| **Interprétation des intentions** | L’agent lit votre saisie en langage naturel et identifie le concept ou l’objectif sous-jacent. Par exemple, une requête sur « personnes en Californie » est interprétée comme une requête d’attribut géographique, et non comme une correspondance de chaîne littérale. L’agent mappe vos expressions à des concepts équivalents sémantiquement qui peuvent apparaître sous différents noms dans vos schémas. |
| **Portée de la recherche** | L’agent effectue une recherche dans les schémas XDM, les jeux de données et les métadonnées de champ disponibles dans votre organisation IMS actuelle et votre sandbox. Il prend en compte les noms de champ, les noms d’affichage, les descriptions et les associations d’utilisation pour trouver les candidats qui correspondent à votre intention. |
| **Classement** | L’agent classe les résultats par pertinence sémantique (à quel point un champ correspond à votre intention déclarée), complétée par des signaux tels que l’exhaustivité des métadonnées et l’utilisation des champs dans votre écosystème de données. Les champs avec des noms descriptifs, des métadonnées renseignées et une utilisation confirmée dans les jeux de données actifs sont mieux classés que les champs qui existent uniquement dans une définition de schéma. L&#39;agent n&#39;expose pas les poids spécifiques affectés à des signaux individuels. |

## Comprendre vos résultats {#understand-your-results}

L&#39;agent de découverte de champ renvoie un jeu de résultats structuré pour chaque requête. Comprendre les composants d’un résultat vous permet d’évaluer les champs candidats et d’agir sur ceux-ci en toute confiance, sans essai ni erreur supplémentaire.

Traitez un champ comme prêt à l’emploi lorsque son libellé **[!UICONTROL Pertinence]** est **[!UICONTROL Très pertinent]**, ses valeurs d’échantillon correspondent aux données attendues (le cas échéant) et que son **[!UICONTROL Contextes d’utilisation]** s’aligne sur la manière dont vous prévoyez de l’utiliser. Si les résultats sont seulement **[!UICONTROL Modérément pertinents]** ou **[!UICONTROL Pertinents]**, si les exemples de valeurs ne correspondent pas à vos attentes ou si le contexte d’utilisation est limité, affinez votre requête et passez en revue un nouveau jeu de résultats avant de continuer.

### Libellés de pertinence

L’agent de découverte de champ attribue un libellé de pertinence dans la colonne **[!UICONTROL Pertinence]** du panneau **[!UICONTROL Champs identifiés]** pour chaque résultat de champ, indiquant à quel point le champ correspond à votre requête.

- **[!UICONTROL Très pertinent]** — Le champ correspond fortement à votre concept déclaré en fonction de son nom, de ses métadonnées et de ses signaux d’utilisation. Confirmez le chemin du champ et passez en revue ses exemples de valeurs pour vérifier qu’il contient les données attendues.
- **[!UICONTROL Modérément pertinent]** — Le champ a un chevauchement sémantique partiel avec votre requête, mais peut différer par sa portée, son type de données ou sa spécificité. Examinez les exemples de valeurs et le contexte d’utilisation pour déterminer s’ils répondent à vos besoins avant de les sélectionner.
- **[!UICONTROL Pertinent]** — Le champ correspond partiellement à votre requête. Il peut partager un chevauchement sémantique mais différer par sa portée, sa spécificité ou son type de données. Examinez les exemples de valeurs et le contexte d’utilisation avant de décider de son utilisation.

Si tous les résultats sont libellés **[!UICONTROL Modérément pertinent]** ou **[!UICONTROL Pertinent]** plutôt que **[!UICONTROL Très pertinent]**, votre requête peut être trop large ou utiliser une terminologie qui ne correspond pas à vos métadonnées de schéma. Affinez votre invite avec des termes de langue ou de domaine plus spécifiques qui reflètent le nom de vos champs.

### Exemples de valeurs

Outre chaque suggestion de champ, l’agent de découverte de champ présente des exemples de valeurs extraits des données du champ dans votre sandbox. Les exemples de valeurs vous permettent de vérifier qu’un champ contient le type de données attendu avant de le sélectionner.

>[!IMPORTANT]
>
>Les exemples de valeurs peuvent contenir des informations d’identification personnelles. Ne les partagez pas en dehors de workflows internes sécurisés.

Les exemples de valeurs ne sont visibles que pour les champs dans les autorisations d’accès aux jeux de données. Pour plus d’informations sur la gouvernance des données et les restrictions d’utilisation dans Experience Platform, consultez la [présentation de la gouvernance des données](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/home).

Si aucune valeur d’exemple n’apparaît pour un champ, il se peut que le champ soit vide dans votre sandbox actuel ou que vos autorisations n’incluent pas l’accès à son jeu de données sous-jacent. Les champs à cardinalité élevée (tels que les champs d’identifiant ou d’UUID) peuvent également ne pas renvoyer de valeurs d’échantillon représentatives. Les valeurs d’échantillon sont agrégées et basées sur la fréquence. Elles ne sont pas traçables par profils individuels.

### Contexte d’utilisation

Chaque résultat de champ comprend un contexte d’utilisation indiquant où le champ apparaît dans votre écosystème de données :

**Schéma De → De Destination Du Jeu De Données Audience → →**

Un champ utilisé dans une audience publiée, qui apparaît dans un jeu de données actif, qui est mappé à une destination active et qui est défini dans un schéma a démontré une utilisation réelle dans votre environnement. Cela permet de distinguer les champs qui sont activement utilisés des champs qui n’existent que dans une définition de schéma, mais qui n’ont pas été utilisés dans la pratique. Utilisez ce signal avec le libellé de pertinence et les valeurs d’échantillon pour effectuer une sélection de champ plus éclairée.

### Résultats dans l’assistant AI

L’agent de découverte de champ renvoie des résultats dans un panneau **[!UICONTROL Champs identifiés]** dans la réponse de l’assistant AI. Le panneau affiche un tableau à trois colonnes :

- **[!UICONTROL Nom du champ]** — Chemin XDM du champ candidat.
- **[!UICONTROL Pertinence]** — Libellé de pertinence attribué au champ (**[!UICONTROL Très pertinent]**, **[!UICONTROL Modérément pertinent]** ou **[!UICONTROL Pertinent]**)
- **[!UICONTROL Contextes d’utilisation]** — Liens indiquant où le champ apparaît dans votre écosystème de données. Sélectionnez **[!UICONTROL audience]**, **[!UICONTROL jeu de données]**, **[!UICONTROL destination]** ou **[!UICONTROL schéma]** pour ouvrir un panneau latéral indiquant où le champ est utilisé.

![Panneau Champs identifiés dans l’assistant AI affichant les lignes de champs candidats avec les libellés de pertinence et les liens Contextes d’utilisation.](./images/field-discovery/fields-identified-panel-in-chat.png)

Une section **[!UICONTROL Résultats expliqués]** s’affiche sous le tableau **[!UICONTROL Champs identifiés]** et fournit un contexte supplémentaire au niveau du champ, y compris des explications et des détails annexes pour chaque résultat. Pour obtenir des conseils sur la navigation dans l’interface de l’assistant AI, consultez le guide [IU de l’assistant AI](../ai-assistant/ai-assistant-ui.md).

## Utiliser l’agent de découverte de champ {#use-field-discovery-agent}

Vous interagissez avec l’agent de découverte de champ par le biais de l’assistant AI en langage naturel. L’agent requiert une déclaration d’intention claire : une requête vague ou trop brève produit des résultats de qualité inférieure ou peut ne pas appeler l’agent de découverte de champ du tout.

Pour la découverte de champs explicite, suivez ce workflow : identifier l’attribut ou le problème de mappage, envoyer une requête de recherche de champ, consulter les résultats classés et le contexte d’utilisation dans le panneau **[!UICONTROL Champs identifiés]**, sélectionner le chemin **[!UICONTROL Nom du champ]** qui correspond à votre intention et appliquer ce chemin XDM dans le créateur de segments, Query Service ou un autre workflow.

Pour utiliser l&#39;agent de détection de champ :

1. Accédez à **[!UICONTROL Assistant AI]** à partir de n’importe quelle application Experience Platform activée. L’espace de travail **[!UICONTROL Assistant IA]** s’affiche.
2. Indiquez explicitement votre intention dans le champ de saisie. Décrivez le concept, l’objectif ou la caractéristique de champ que vous recherchez. Par exemple : *« Rechercher des champs liés au statut de désinscription aux e-mails du client.«*
3. Examinez les résultats avec classement dans le panneau **[!UICONTROL Champs identifiés]**. Chaque ligne comprend un libellé de pertinence et un chemin d’accès au champ XDM dans la colonne **[!UICONTROL Nom du champ]**.
4. Sélectionnez **[!UICONTROL audience]**, **[!UICONTROL jeu de données]**, **[!UICONTROL destination]** ou **[!UICONTROL schéma]** dans la colonne **[!UICONTROL Contextes d’utilisation]** pour ouvrir un panneau latéral indiquant où le champ est utilisé. Pour plus de contexte au niveau du champ, reportez-vous à la section **[!UICONTROL Résultats expliqués]** située sous le tableau des résultats.

   ![Panneau latéral dans l’assistant AI affichant les contextes d’utilisation d’un champ sélectionné, y compris les associations d’audience, de jeu de données, de destination et de schéma.](./images/field-discovery/fields-identified-panel-expanded.png)

5. Utilisez le chemin d’accès **[!UICONTROL Nom du champ]** dans les outils en aval tels que le créateur de segments, Query Service ou les workflows d’ingestion de données, selon votre cas d’utilisation. L’agent de découverte de champ fournit la référence de champ, mais ne l’insère pas dans d’autres outils.

Si nécessaire, sélectionnez le menu déroulant **[!UICONTROL Raisonnement terminé]** au-dessus de la réponse pour confirmer que l’agent de découverte de champ a géré votre requête. La liste déroulante affiche les détails du raisonnement qui indiquent l’agent appelé.

>[!NOTE]
>
>Si le panneau de raisonnement n&#39;indique pas l&#39;agent de découverte de champs, votre requête peut ne pas avoir contenu une intention de découverte de champs claire. Reformulez votre requête avec un langage de recherche de champ explicite et renvoyez-la. Voir [Dépannage](#troubleshooting) pour les problèmes d’appel courants.

Pour plus d’informations sur l’interface de l’assistant IA, consultez le guide de l’interface utilisateur de l’assistant [IA](../ai-assistant/ai-assistant-ui.md).

## Cas d’utilisation pris en charge {#supported-use-cases}

Les sections suivantes décrivent chacune des trois fonctions de Field Discovery Agent avec des scénarios représentatifs et des exemples d&#39;invites. Les résultats incluent des libellés de pertinence et un contexte d’utilisation pour aider à évaluer les champs. Pour l’interprétation des résultats, voir [Comprendre vos résultats](#understand-your-results). L&#39;agent de découverte de champ renvoie uniquement des informations de champ — il ne crée pas d&#39;audiences, n&#39;exécute pas de requêtes et ne transmet pas de données à d&#39;autres outils. Après avoir identifié un champ, lisez son chemin XDM dans la colonne **[!UICONTROL Nom du champ]** et utilisez-le dans votre workflow en aval.

### Identification des champs d’un concept d’entreprise

Lorsque vous décrivez un concept ou un attribut de données spécifique, l’agent de découverte de champs renvoie une liste classée de champs qui correspondent sémantiquement à votre description.

> « Quels champs représentent l’État d’origine ou la province d’un client ? »
> « Rechercher les champs liés à la date de transaction d&#39;achat. »
> « Quels champs contiennent des informations sur le consentement de marketing par e-mail ? »

La réponse répertorie les champs candidats avec leur libellé de pertinence et leur chemin XDM dans le panneau **[!UICONTROL Champs identifiés]**. Les champs libellés **[!UICONTROL Très pertinent]** correspondent le mieux à votre concept déclaré. Si les meilleurs résultats sont intitulés **[!UICONTROL Modérément pertinent]** ou **[!UICONTROL Pertinent]** plutôt que **[!UICONTROL Très pertinent]**, affinez votre requête en utilisant une terminologie plus spécifique ou un contexte au niveau du champ.

### Obtention de recommandations de champs pour un cas d’utilisation

Lorsque vous décrivez un objectif ou un cas d’utilisation de workflow, comme la création d’un segment, l’intégration d’un jeu de données ou la préparation d’une requête, l’agent de découverte de champ recommande des champs alignés sur cet objectif, hiérarchisés par pertinence.

> « Je veux constituer une audience de clients à forte valeur ajoutée. Quels champs dois-je utiliser ? »
> « Champs recommandés pour la modélisation de la propension à l’achat. »
> « Quels champs dois-je inclure lors de l’intégration d’un jeu de données de transaction de vente au détail ? »

La réponse renvoie une liste de champs prioritaires avec un contexte de pertinence. Examinez le contexte d’utilisation de chaque champ recommandé pour confirmer qu’il est activement utilisé dans votre environnement.

### Enrichir le contexte du champ

Lorsque vous demandez des informations sur un champ spécifique par nom ou chemin d’accès, l’agent de découverte de champ renvoie un contexte détaillé pour ce champ, y compris des exemples de valeurs, l’emplacement du schéma et l’utilisation dans les jeux de données, les audiences et les destinations.

> « En savoir plus sur le champ `person.name.lastName`. »
> « Quels exemples de valeurs existent pour `homeAddress.stateProvince` ? »
> « Où se trouve le champ `commerce.purchases.value` utilisé dans mes jeux de données et mes audiences ? »

La réponse renvoie les exemples de valeurs du champ, l’emplacement du schéma, les jeux de données associés et les audiences ou destinations où le champ apparaît. Examinez ce contexte pour confirmer que le champ contient les données attendues.

## Dans la portée et hors de la portée {#in-scope-and-out-of-scope}

Cette section résume ce que l&#39;agent de découverte de champs peut et ne peut pas faire. Pour obtenir des conseils détaillés sur les tâches, voir [Cas d’utilisation pris en charge](#supported-use-cases). Pour les contraintes de plateforme, voir [ Mécanismes de sécurisation et limitations ](#guardrails-and-limitations).

### Dans la portée

La liste suivante décrit les tâches que l’agent de découverte de champ peut effectuer ; utilisez-le pour confirmer que l’agent peut répondre à votre demande avant de vous y fier dans votre workflow.

- Identifier les champs XDM qui correspondent à un concept commercial ou à une description en langage naturel.
- Champs recommandés pour un objectif ou un cas d’utilisation de workflow déclaré.
- Enrichir un champ spécifique avec des exemples de valeurs, l’emplacement du schéma et le contexte d’utilisation.
- Résultats renvoyés classés par pertinence sémantique, classés comme Très pertinent, Modérément pertinent ou Pertinent.
- Affichage des exemples de valeurs dans vos autorisations de jeux de données.

### Hors de portée

La liste suivante décrit les actions que l’agent de découverte de champ n’effectue pas ; utilisez-le pour éviter de dépendre de l’agent pour le travail en dehors de sa portée.

- Modifier des schémas, des jeux de données, des champs ou des audiences.
- Créez ou publiez des audiences ou des segments.
- Exécutez des requêtes ou activez des données vers des destinations.
- Accédez aux champs ou aux jeux de données en dehors de vos autorisations autorisées.
- Exposez la logique d’incorporation interne, l’architecture de base de données vectorielle ou les détails d’implémentation de liaison d’entités.
- Garantissez un intervalle de temps spécifique pour les mises à jour de la base de connaissances après des modifications de schéma ou de jeu de données.

## Mécanismes de sécurisation et limitations {#guardrails-and-limitations}

Ces mécanismes de sécurisation sont importants, car Field Discovery Agent fonctionne dans des contraintes au niveau de la plateforme qui affectent la disponibilité et la qualité des résultats. Utilisez-les pour interpréter les résultats manquants, retardés ou incomplets et pour résoudre les écarts inattendus avec des attentes réalistes.

### Base de connaissances

Field Discovery Agent repose sur une base de connaissances qui est régulièrement actualisée avec le schéma et les métadonnées de votre environnement Experience Platform. Les résultats reflètent l’état de la base de connaissances au moment de votre requête, et non l’état en temps réel de vos schémas, et il peut y avoir un délai entre l’ingestion des données et le moment où elles sont affichées dans l’agent.

Les nouveaux schémas, champs ou jeux de données ajoutés à votre environnement peuvent ne pas apparaître immédiatement dans les résultats de l’agent Field Discovery. Les résultats peuvent prendre du temps pour refléter les changements récents.

>[!NOTE]
>
>L&#39;intervalle d&#39;actualisation de la base de connaissances peut changer. Si un champ récemment ajouté n’apparaît pas dans les résultats, attendez que la base de connaissances se mette à jour, puis soumette à nouveau votre requête.

### Qualité et couverture des métadonnées

La qualité des résultats dépend de la qualité et de l’exhaustivité des métadonnées de champ dans votre environnement Experience Platform. L’agent utilise les noms de champ, les noms d’affichage, les descriptions et les associations d’utilisation pour classer les résultats. Les champs contenant des métadonnées manquantes ou de mauvaise qualité peuvent ne pas apparaître dans les résultats ou se classer plus bas que prévu.

Si vous disposez d’un accès en modification de schéma, vous pouvez améliorer la qualité des résultats en :

- Utilisation de noms d’affichage clairs et descriptifs pour les champs de vos schémas.
- Ajoutez des descriptions de champ si possible.
- Association de champs aux jeux de données actifs plutôt que de les laisser comme définitions de schéma uniquement.

Pour obtenir des conseils sur la modification des noms d’affichage des champs et des descriptions dans l’éditeur de schémas, consultez [Création et modification de schémas dans l’interface utilisateur](https://experienceleague.adobe.com/fr/docs/experience-platform/xdm/ui/resources/schemas).

Si vous ne disposez pas de l’accès nécessaire à la modification des schémas et que les résultats sont systématiquement médiocres, contactez votre administrateur Experience Platform ou votre équipe d’ingénierie de données pour consulter les métadonnées de champ des schémas que vous utilisez.

### Contraintes d’accès et de PII

L’agent de découverte de champ respecte tous les contrôles d’accès Experience Platform existants et fonctionne dans votre contexte de sandbox actuel. Vous ne recevez des résultats que pour les champs des schémas et des jeux de données auxquels vous êtes autorisé à accéder.

Les exemples de valeurs sont régis par les mêmes autorisations au niveau du jeu de données. Les champs des jeux de données activés pour le profil avec des restrictions PII renvoient des valeurs d’exemple uniquement si vous disposez de l’accès requis. Voir [Exemples de valeurs](#sample-values) pour des conseils de gestion. L’agent de découverte de champ ne contourne pas les restrictions d’accès activées au niveau du champ ou du profil.

## Bonnes pratiques {#best-practices}

Suivez les conseils ci-après pour obtenir des résultats précis et exploitables de la part de l&#39;agent Field Discovery.

- **Soyez précis sur le concept, pas seulement sur le type de champ.** Une invite telle que « trouver un champ d’état » produit des résultats de qualité inférieure à « trouver le champ qui contient l’état des États-Unis d’un client pour la segmentation géographique ». La spécificité donne à l’agent davantage de signal à comparer à vos métadonnées. Consultez [Fonctionnement de l’agent de découverte de champ](#how-field-discovery-agent-works) pour en savoir plus sur l’importance.
- **Utilisez une terminologie correspondant aux métadonnées de votre schéma.** Si vos schémas utilisent le terme « transaction » plutôt que « achat », utilisez « transaction » dans vos invites. L’agent correspond aux noms et descriptions de champ réels, et pas seulement à des concepts généraux.
- **Vérifier les champs avant la validation.** Après avoir trouvé des champs candidats, demandez des informations sur un champ spécifique par nom ou chemin d’accès afin de passer en revue ses exemples de valeurs et son contexte d’utilisation avant de l’utiliser dans un segment ou une requête. Vous réduisez ainsi le risque de sélectionner le mauvais champ.
- **Itérez lorsque les résultats sont modérément pertinents ou pertinents plutôt que très pertinents.** Reformulez votre requête avec une terminologie différente ou ajoutez plus de contexte à propos de votre cas d’utilisation. Une deuxième requête, plus spécifique, fait souvent apparaître de meilleurs candidats.
- **Incluez le contexte de la portée dans vos invites.** Pour la segmentation géographique, incluez la région cible. Pour les requêtes temporelles, incluez l’attribut time. Plus vous fournissez de contexte, plus le classement des résultats est ciblé.

## Exemples d’invites {#example-prompts}

Utilisez cette section comme bibliothèque d’invites de référence rapide. Si vous découvrez l&#39;agent Field Discovery, lisez d&#39;abord [Bonnes pratiques](#best-practices) et [Cas pratiques pris en charge](#supported-use-cases) pour comprendre quand et pourquoi chaque fonction s&#39;applique.

### Invites d’identification

Utilisez ces invites lorsque vous connaissez le concept de données dont vous avez besoin, mais pas le champ qui le contient.

> « Quel champ contient l’état ou la région d’un client ? »
> « Recherchez les champs liés au statut d’abonnement aux e-mails. »
> « Quel champ contient la date du premier achat d’un client ? »
> « Identifier les champs qui représentent la valeur de la durée de vie du client. »
> « Quels champs de mon schéma de profil sont liés à l’appartenance au programme de fidélité ? »

### Invites de recommandation

Utilisez ces invites lorsque vous démarrez un workflow et que vous avez besoin de conseils sur les champs à inclure pour un objectif spécifique.

> « Quels champs dois-je utiliser pour créer une audience de réengagement ? »
> « Champs recommandés pour une audience ciblant des clients qui n’ont pas effectué d’achats depuis 90 jours. »
> « Quels champs sont les plus utiles pour modéliser le risque de résiliation ? »
> « Suggérer des champs à inclure lors de la création d’une segmentation géographique. »
> « Je suis en train de créer un modèle de propension à acheter. Avec quels champs dois-je commencer ? »

### Invites d’enrichissement

Utilisez ces invites lorsqu&#39;un champ candidat est en attente de vérification avant de l&#39;utiliser dans un segment, une requête ou un mappage.

> « Parlez-moi de `homeAddress.stateProvince`. »
> « Afficher les exemples de valeurs pour `commerce.purchases.value`. »
> « Où est-`person.name.lastName` utilisé dans mes jeux de données et mes audiences ? »
> « Quels jeux de données contiennent les `web.webPageDetails.URL` de champ ? »
> « Est-`segmentMembership` mappé à des destinations actives ? »

## Résolution des problèmes {#troubleshooting}

Utilisez cette section lorsque des résultats sont manquants, inattendus ou lorsque vous ne savez pas si l&#39;agent de découverte de champ a géré votre demande.

- **Un champ récemment ajouté n’apparaît pas dans les résultats.** La base de connaissances peut ne pas encore refléter le nouveau schéma ou champ. Patientez le temps que la base de connaissances se mette à jour après l’ajout de schémas ou de champs à votre environnement, puis soumettez à nouveau votre requête. Voir [Base de connaissances](#knowledge-base).

- **Tous les résultats sont étiquetés Modérément pertinent ou Pertinent plutôt que Très pertinent.** Votre requête est peut-être trop large ou la terminologie que vous avez utilisée ne correspond peut-être pas à vos métadonnées de champ. Affinez votre invite avec une langue plus spécifique ou des termes qui correspondent à la manière dont vos champs sont nommés dans vos schémas. Voir [ Bonnes pratiques ](#best-practices).

- **L&#39;agent Field Discovery n&#39;a pas été appelé.** Vous avez envoyé une requête dans l’assistant AI, mais le panneau **[!UICONTROL Raisonnement terminé]** n’indique pas l’agent de découverte de champ. Votre requête ne contenait peut-être pas une intention de découverte de champ claire. Reformulez explicitement votre requête, par exemple, « Rechercher le champ qui contient le statut d’opt-out des e-mails du client », puis soumettez-la à nouveau. Voir [ Utilisation de l’agent de découverte de champ ](#use-field-discovery-agent).

- **Les exemples de valeurs ne s’affichent pas pour un champ.** Le champ peut être vide dans votre sandbox actuel, vos autorisations peuvent ne pas inclure l’accès à son jeu de données sous-jacent ou le champ peut avoir une cardinalité élevée (par exemple un champ d’identifiant) pour lequel les exemples de valeurs ne sont pas affichés. Confirmez vos autorisations d’accès au jeu de données et vérifiez que le champ est rempli de données. Voir [Contraintes d’accès et d’informations d’identification personnelles](#access-and-pii-constraints).

- **Les résultats incluent les champs des schémas auxquels vous ne vous attendiez pas.** L’agent de découverte de champ recherche tous les schémas et jeux de données de votre sandbox actuel qui sont accessibles avec vos autorisations. Si des résultats inattendus s’affichent, confirmez votre contexte de sandbox actif dans l’assistant AI et vérifiez quels schémas et jeux de données sont accessibles à votre rôle.

Pour vérifier quel agent a géré votre requête, reportez-vous à l’étape 6 de la section [Utiliser l’agent de découverte de champ](#use-field-discovery-agent).
