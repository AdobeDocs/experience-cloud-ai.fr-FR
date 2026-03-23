---
title: Adobe Marketing Agent for Microsoft 365 Copilot
description: Découvrez comment utiliser Adobe Marketing Agent for Microsoft 365 Copilot.
hide: true
hidefromtoc: true
source-git-commit: 224c38c54ff1cf73abdb5eca5f0961b41a1daefc
workflow-type: tm+mt
source-wordcount: '1793'
ht-degree: 0%

---

# Adobe Marketing Agent pour [!DNL Microsoft 365 Copilot]

Adobe Marketing Agent for [!DNL Microsoft 365 Copilot] est un outil optimisé par l’IA qui connecte Adobe Experience Platform directement à [!DNL Microsoft 365 Copilot]. Avec cet agent, vous pouvez poser des questions en langage naturel dans [!DNL Microsoft 365] applications telles que [!DNL Teams], [!DNL Word], [!DNL Powerpoint] et [!DNL Excel] pour récupérer instantanément des informations marketing d’Experience Platform sans interrompre votre workflow. Le même agent est disponible sur toutes ces applications, et votre historique de conversation avec Adobe Marketing Agent est reporté. Vous pouvez donc commencer à effectuer des recherches dans [!DNL Copilot] en [!DNL Teams], par exemple, et poursuivre la conversation en [!DNL Word] ou en [!DNL Powerpoint] pendant que vous rédigez un résumé de campagne ou passez en revue une présentation.

Avec Adobe Marketing Agent for [!DNL Microsoft 365 Copilot], les responsables marketing, les équipes d’analyse et d’informations et les parties prenantes peuvent :

- Prenez plus rapidement des décisions de marketing axées sur les données.
- Réduisez le temps nécessaire pour passer d’un outil à un autre.
- Simplifiez l’accès aux informations sur les audiences et les parcours entre les équipes.

## Fonctionnement de l’agent

>[!IMPORTANT]
>
>Adobe Marketing Agent for [!DNL Microsoft 365 Copilot] prend actuellement en charge Experience Platform Operational Insights, Customer Journey Analytics Data Insights, Audience Agent et Journey Agent.

Adobe Marketing Agent for [!DNL Microsoft 365 Copilot] offre une expérience intégrée entre Experience Platform et les applications [!DNL Microsoft 365] :

- Adobe Marketing Agent apparaît en tant qu’agent dans [!DNL Microsoft 365 Copilot], y compris dans [!DNL Teams], [!DNL Word], [!DNL Powerpoint] et [!DNL Excel].
- Connectez-vous avec votre compte Adobe et sélectionnez l’environnement de données (sandbox, vue de données) que vous souhaitez utiliser.

### Accès aux données et autorisations

Les réponses que vous recevez reflètent les **données et niveau d’accès** liés à votre identité Adobe. Ce que vous pouvez interroger et voir est le même que ce à quoi vous avez droit dans Experience Platform et ses solutions associées. Le Adobe Marketing Agent **hérite** de ces autorisations et ne nécessite **pas** une configuration d’autorisations distincte pour l’intégration [!DNL Microsoft 365]. Pour les fonctionnalités sous-jacentes de l’assistant Experience Platform AI et d’autres agents Adobe AI, les exigences d’autorisation **autorisation sont inchangées** relatives à l’utilisation de ces fonctionnalités dans Experience Platform.

L’agent connecte votre instance [!DNL Microsoft 365] à Experience Platform et à ses applications associées (Real-Time CDP, Adobe Journey Optimizer et Customer Journey Analytics). Grâce à cette intégration, vous pouvez ensuite utiliser l’assistant et les agents Experience Platform AI pour récupérer des informations pertinentes directement sur votre instance [!DNL Microsoft 365]. Les réponses renvoyées dans votre instance [!DNL Microsoft 365] sont présentées sous la forme de textes, tableaux et visualisations de données en langage conversationnel et naturel. De plus, la prise en charge des questions et investigations de suivi est disponible dans la même conversation [!DNL Copilot].

## Cas d’utilisation clés et exemples de scénarios

| Cas d’utilisation | Description |
| --- | --- |
| Récupérer des informations opérationnelles pour les audiences et les parcours client | Avec Adobe Marketing Agent, vous pouvez facilement récupérer des informations opérationnelles sur vos audiences et parcours clients. Vous pouvez identifier les audiences les plus importantes ou les plus engagées afin de déterminer les priorités sur lesquelles concentrer vos efforts. Vous pouvez identifier les parcours clients actuellement actifs et en apprendre davantage sur leurs performances, ce qui vous permet d’identifier les opportunités d’optimisation. L’agent vous permet également de suivre la croissance ou le rétrécissement de vos différents segments au fil du temps, ce qui vous permet de répondre aux modifications de la dynamique de votre audience au fur et à mesure qu’elles se produisent. |
| Utiliser la visualisation des données pour mieux analyser les parcours et les campagnes des clients | Vous pouvez examiner les performances du parcours et les abandons, comparer les performances des campagnes au fil du temps et déterminer les points de contact qui génèrent les conversions. De plus, vous pouvez générer des rapports visuels sur les performances des campagnes et les comparer sur plusieurs canaux, régions ou sur différentes périodes. Vous pouvez également explorer les tendances sans avoir à créer manuellement de requêtes ou de tableaux de bord. |
| Favoriser la collaboration et la prise de décisions | Utilisez les invites suggérées pour explorer les audiences, les campagnes et le trafic web. Tirez parti d’une interface en langage naturel pour apprendre plus facilement les concepts Experience Platform et Customer Journey Analytics. De plus, vous pouvez partager des informations sur les canaux de [!DNL Teams] ou les conversations lors des réunions de planification. Vous pouvez également utiliser Adobe Marketing Agent pour répondre à des questions ad hoc en temps réel lors de l’examen des plans ou des présentations, ce qui vous permet de maintenir l’alignement des parties prenantes sur le même ensemble de mesures et de définitions. |

## Conditions préalables

Avant de pouvoir utiliser Adobe Marketing Agent pour [!DNL Microsoft 365 Copilot], vous devez d’abord vous assurer que vous disposez des éléments suivants :

- [!DNL Microsoft 365] avec [!DNL Microsoft Teams] ou [!DNL Microsoft Copilot Chat].
- Experience Platform et au moins l’un des éléments suivants : Real-Time CDP, Adobe Journey Optimizer et/ou Customer Journey Analytics.
- Droit à l’Experience Platform Agent Orchestrator et aux agents.
- Accès au compte Adobe Experience Cloud de votre entreprise (droits de connexion et de produit) pour les solutions et les données que vous utilisez. Si vous ne disposez pas d’un accès à Adobe, contactez votre administrateur Adobe.

## Activez l’agent pour votre organisation {#enable-the-agent-for-your-organization}

Les utilisateurs finaux ne peuvent utiliser le Adobe Marketing Agent qu’après sa mise à disposition dans votre client [!DNL Microsoft 365]. **Contactez votre administrateur [!DNL Microsoft 365] Copilot** (ou un administrateur équivalent pour les agents Copilot de votre organisation) pour activer l&#39;accès et affecter l&#39;agent selon les besoins de votre organisation.

Les résultats standard après la configuration de l’administration incluent :

- Vous pouvez ouvrir **[!DNL Agent Store]** dans [!DNL Teams], trouver des **[!DNL Adobe Marketing Agent]** dans votre liste d&#39;agents et choisir **[!DNL Add]** les joindre à vos agents Copilot.
- Votre administrateur Copilot peut également **publier** l’agent pour tous les membres de votre organisation ou pour des groupes spécifiques, de sorte que les utilisateurs n’aient pas besoin de l’ajouter individuellement.

Pour connaître les étapes d’administration et les options de politique dans le centre d’administration [!DNL Microsoft 365], consultez [Gérer les agents pour le copilote Microsoft 365](https://learn.microsoft.com/en-us/microsoft-365-copilot/extensibility/manage) dans la documentation de Microsoft.

## Commencer

Une fois que votre organisation a activé l’agent (voir [Activer l’agent pour votre organisation](#enable-the-agent-for-your-organization)), accédez à [!DNL Microsoft 365 Copilot] dans l’application de votre choix et utilisez le volet de navigation de gauche pour sélectionner **[!DNL All Agents]**.

![Volet de navigation de gauche du copilote Microsoft 365 avec tous les agents sélectionnés.](../agents/images/ama/all-agents.png)

Recherchez la carte à [!DNL Adobe Marketing Agent] ou utilisez la barre de recherche pour rechercher manuellement l’agent. Une fois que vous disposez de l’agent, sélectionnez la carte.

![Carte Adobe Marketing Agent ou résultat de la recherche dans la galerie d&#39;agents.](../agents/images/ama/select-ama.png)

Utilisez la fenêtre pop-up pour en savoir plus sur l’agent. Lorsque vous êtes prêt, sélectionnez **[!DNL Add]**.

Fenêtre contextuelle de détails de ![Adobe Marketing Agent avec le bouton Ajouter en surbrillance.](../agents/images/ama/add-ama.png)

Le tableau de bord [!DNL Microsoft 365 Copilot] est mis à jour avec l’identité graphique [!DNL Adobe Marketing Agent] désormais sur la page principale.

![Page d&#39;accueil du copilote Microsoft 365 affichant Adobe Marketing Agent sur le tableau de bord principal.](../agents/images/ama/home.png)

### Connexion et définition du contexte

Ensuite, demandez à l’agent de se connecter et de suivre les étapes suivantes requises pour authentifier votre compte. Au cours de cette étape, vous devez copier un code numérique renvoyé par l’agent, puis vous connecter à votre organisation Adobe. Si vous ne pouvez pas vous connecter complètement ou si vous n’avez pas accès aux solutions Adobe pour votre organisation, contactez votre **administrateur Adobe**.

![Étape de connexion à Adobe présentant un code numérique à copier et des instructions pour s’authentifier auprès de votre organisation Adobe.](../agents/images/ama/sign-in.png)

En cas de réussite, utilisez le définisseur de contexte pour établir la source de documentation, le sandbox et la vue de données que vous utiliserez pour vos requêtes.

![Interface utilisateur du définisseur de contexte pour choisir la source de documentation, le sandbox et la vue de données pour les requêtes.](../agents/images/ama/context.png)

### Utiliser l’agent pour récupérer des informations opérationnelles

Une fois connecté, vous pouvez utiliser les invites fournies dans la page principale pour commencer. Vous pouvez également utiliser une invite de démarrage qui permet d’analyser les audiences marketing, de passer en revue les performances des campagnes et de surveiller les parcours des campagnes. Par exemple, sélectionnez **[!DNL Review campaign performance]** puis **[!DNL Analyze engagement - Show web visitors for top 10 products last week]**.

![Des invites de démarrage sur la page d&#39;accueil de l&#39;agent, incluant la vérification des performances de la campagne et l&#39;analyse des options d&#39;engagement.](../agents/images/ama/starter-guide.png)

Patientez quelques instants le temps que l’agent calcule, puis il répond avec une représentation visualisée de vos données. Vous pouvez utiliser le graphique à barres présenté ou sélectionner **[!DNL View data]** pour afficher les données dans les tableaux.

![Réponse de l’agent avec un graphique à barres permettant de visualiser les visiteurs web pour les principaux produits et l’option Afficher les données ](../agents/images/ama/response.png).

![Mêmes informations affichées qu’un tableau de données après avoir sélectionné Afficher les données.](../agents/images/ama/tables.png)

Vous pouvez approfondir vos recherches en sélectionnant les questions de suivi recommandées par l’agent. Vous pouvez également permuter et essayer différentes invites de démarrage, vérifier les sources d&#39;informations référencées par l&#39;agent ou fournir un feedback en utilisant le mécanisme de feedback.

![Questions de suivi suggérées sous la réponse de l&#39;agent pour une enquête plus approfondie.](../agents/images/ama/follow-up.png)

Pour plus d’informations sur les fonctionnalités de l’interface utilisateur de l’assistant AI, consultez le guide sur [l’utilisation de l’assistant AI](../ai-assistant/ai-assistant-ui.md).

## Sécurité, confidentialité et IA responsable

**Gestion et gouvernance des données**

Le Adobe Marketing Agent repose sur les mêmes contrôles et la même gouvernance que ceux qui s’appliquent à Experience Platform et à [!DNL Microsoft 365]. Votre entreprise conserve la propriété et le contrôle de ses données. Les informations renvoyées par l’intermédiaire de l’agent sont limitées aux autorisations Adobe et aux droits de données de chaque utilisateur ; aucun modèle d’autorisation supplémentaire n’est introduit pour la surface [!DNL Microsoft 365] au-delà de ce qui s’applique déjà dans Experience Platform et les agents Adobe AI associés.

**Utilisation responsable de l’IA**

L’agent est destiné à renvoyer des informations en lecture seule et ne modifie pas les données de vos clients dans Experience Platform. Vous devez examiner les résumés et analyses générés avant de les utiliser pour prendre des décisions commerciales.

**Langues et portée prises en charge**

La version initiale est disponible en tant qu’expérience en anglais. Les fonctionnalités sont limitées à des informations en lecture seule ; l’agent ne crée ni ne met à jour de ressources marketing ou de configurations.

## Annexe

Lisez ce qui suit pour plus d’informations sur Adobe Marketing Agent for [!DNL Microsoft 365 Copilot].

### Étapes d’administration de Adobe Marketing Agent [!DNL Microsoft 365 Copilot]

Pour configurer des agents provenant d’un fournisseur externe (développeurs tiers ou marché commercial Microsoft), vous devez d’abord vous assurer que les paramètres de votre client autorisent les applications externes, puis les gérer via la section Applications ou agents intégrés du centre d’administration.

#### Activer les agents externes dans les paramètres du client

Avant de pouvoir déployer des agents externes, la politique de votre organisation doit les autoriser.

- Connectez-vous au centre d’administration [Microsoft 365](https://admin.microsoft.com/).
- Accédez à **Agents** > **Paramètres** > **Accès utilisateur**.
- Sous **Types d’agent autorisés** assurez-vous que **Autoriser les applications et les agents créés par des éditeurs externes** est sélectionné.

>[!IMPORTANT]
>
>Si ce paramètre est désactivé, les agents externes n&#39;apparaîtront pas dans le [magasin d&#39;agents](https://devblogs.microsoft.com/microsoft365dev/introducing-the-agent-store-build-publish-and-discover-agents-in-microsoft-365-copilot/) pour vos utilisateurs.

#### Acquérir et approuver l’agent

En règle générale, vous pouvez trouver des agents externes dans le [[!DNL Microsoft Commercial Marketplace]](https://appsource.microsoft.com/) .

- **Sur la Marketplace** : recherchez l’agent de votre choix et sélectionnez **Get it now**. Vous serez alors souvent redirigé vers la page **Applications intégrées** de votre centre d’administration.
- **Autorisations de révision** : dans la liste [Applications intégrées](https://learn.microsoft.com/en-us/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide), sélectionnez l’agent externe.
- Consultez les onglets **Données et outils** et **Sécurité et conformité** pour identifier les données auxquelles le fournisseur externe aura accès.
- Sélectionnez **Approuver** ou **Activer** pour le déplacer dans l’inventaire de votre organisation.

#### Déployer sur certains utilisateurs

Une fois approuvé, vous pouvez contrôler exactement qui voit l’agent dans sa barre latérale Copilote.

- Dans le [[!DNL Microsoft 365] centre d’administration](https://admin.microsoft.com/), accédez à **Agents** > **Tous les agents**.
- Sélectionnez l’agent externe dans la liste.
- Sélectionnez **Déployer** (ou **Modifier l’affectation**).
- Choisissez **Utilisateurs/groupes spécifiques** et recherchez les individus ou les groupes [!DNL Entra ID] qui doivent l’avoir.
- Sélectionnez **Terminer le déploiement**. L’agent est ainsi « envoyé » à ces utilisateurs pour qu’il apparaisse automatiquement dans leur interface Copilote.

#### Gestion des mises à jour

Les fournisseurs externes mettent fréquemment à jour leurs agents. Pour gérer ces mises à jour, suivez les bonnes pratiques ci-dessous :

- Vérifiez régulièrement le [[!DNL Agent Registry]](https://learn.microsoft.com/en-us/microsoft-365/admin/manage/agent-registry?view=o365-worldwide).
- Si une mise à jour nécessite de nouvelles autorisations, l’agent peut afficher le statut **Mise à jour en attente**.
- Vous devez approuver manuellement **Approuver les mises à jour** avant que la nouvelle version ne soit déployée pour les utilisateurs affectés.