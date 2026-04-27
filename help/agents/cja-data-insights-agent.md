---
description: Découvrez comment visualiser des données avec le Data Insights Agent dans Customer Journey Analytics
title: Visualiser les données avec le Data Insights Agent dans Customer Journey Analytics
role: User, Admin
solution: Customer Journey Analytics
TQID: https://experienceleague.adobe.com/UtKIDlN2x7MOAiHNRRQ8b5OO4fIwzV74r1fnfMwblcQ
product_v2: id: e98b7246-966c-4318-9e95-cad2f7a17dc7
feature_v2: id: b743a5d9-dc51-41ed-8b2f-86a1f8de430fid: c73c4213-d623-4126-81f4-80b42e5e2656id: ce577701-5b9e-4fe4-8fa3-4eedea976da4
subfeature_v2: id: b1f5d324-a668-4e51-a59b-6fc0862d7310id: bc7a5a86-1a70-451f-985c-037b65f091d1id: df7fb1db-aa1b-4314-98ac-59dbfcc3044fid: e44e560d-5e5c-4a5f-9a87-eb8adbb817af
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e1e0219c-f879-479f-8427-888ed2a6e9c2id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: dd7883d8eccab3b0f006d55a850248e1c347d7e7
workflow-type: tm+mt
source-wordcount: 2690
ht-degree: 4%

---

# Visualisation des données avec Data Insights Agent

>[!AVAILABILITY]
>
>Data Insights Agent est disponible pour les clients éligibles pendant une durée limitée. Data Insights Agent est accessible jusqu’au 31 mars 2026. Pour continuer à utiliser Data Insights Agent au-delà de cette date sans interruption, contactez votre représentant de compte Adobe pour en savoir plus sur les licences Adobe Experience Platform Agent Orchestrator.

Data Insights Agent, accessible à partir de l’[assistant AI](/help/ai-assistant/ai-assistant-ui.md), est un agent de conversation IA génératif qui répond rapidement et efficacement aux questions sur vos données. Il crée des visualisations pertinentes dans Analysis Workspace à l’aide de composants de votre vue de données et de vos données réelles.

L’utilisation de Data Insights Agent pour répondre aux questions relatives aux données dans Analysis Workspace peut vous permettre de gagner beaucoup de temps que vous consacreriez autrement à créer manuellement des visualisations dans Analysis Workspace et à vous familiariser avec vos composants de vue de données.

![Data Insights Agent dans l’assistant AI](/help/agents/images/cja-agent/cja-ai-asst-da.gif)

## Fonctionnalités incluses ou non dans la portée

| Fonctionnalité | Dans la portée | Hors de portée |
| --- | --- | --- |
| **Types de visualisation** | <ul><li>Ligne</li><li>Multiligne</li><li>Tableau à structure libre</li><li>Barre</li><li>Anneau</li><li>Nombre de résumés</li></ul> | <ul><li>Flux</li><li>Abandon</li><li>Tableau de cohortes</li><li>Aires, Aires empilées</li><li>Bar Stacked</li><li>Puce</li><li>Combiné</li><li>Histogramme</li><li>Horizontal Bar, Horizontal Bar Stacked</li><li>Key Metric Summary</li><li>Graphique de dispersion</li><li>Summary Change</li><li>Texte</li><li>Treemap</li><li>Venn</li><li>Guided analysis: Active growth, Conversion trends, Engagement, First use impact, Frequency, Funnel, Net growth, Release impact, Retention, Timeline, Trends</li></ul> |
| **Workspace actions and agent capabilities** | <ul><li>Build and update visualizations<p>Generates a freeform table and associated visualization (such as a line, bar, donut, and so forth).</p><p>For example, *What is the profit across SKUs from February to May?*</p></li><li>Ask follow-up questions<p>Respond to a prompt in the context from any prior prompts. Par exemple :</p> <ul><li>Prompt 1: *Trend events from March.*</li><li>Prompt 2: *Show me the data from March to April instead*</li></ul> </li><li>Out-of-scope prompt detection<p>If you submit a prompt that is out of scope, such as *Export this project*, Data Insights Agent responds by informing you that the question is out of scope.</p></li></ul> | <ul><li>Partager</li><li>Exporter</li><li>Télécharger</li><li>Manage user preferences</li><li>Manage data view</li><li>Analytics Dashboards app</li><li>Attribution</li><li>In-line summary or response<p>Data Insights Agent cannot respond in-line in the chat rail with a summary answer of a user prompt. Examples of out-of-scope prompts are, *Give me a summary of the insights from my last prompt* and *Summarize the highlights from the line visualization.*</p></li></ul> |
| **Clarifying questions** | If you ask a question that does not have enough context for Data Insights Agent to answer, or is too generic, Data Insights Agent responds with a clarifying question or suggested options. <p>The following clarifying questions are examples of component-related questions:</p><ul><li>Metric: *Which &quot;revenue&quot; metric did you mean?*</li><li>Dimension : *Sur laquelle des « régions » ci-dessous voulez-vous vous concentrer ?*</li><li>Segment : *Quel segment de « Compte » vouliez-vous appliquer ?*</li><li>Période : *Par « mois dernier », vouliez-vous dire le dernier mois complet ou les 30 derniers jours ?*</li></ul><p>La question de clarification suivante est un exemple de question liée aux éléments de dimension :</p> <ul><li>Quel « nom de magasin » vouliez-vous dire ? (par exemple, #5274 de magasin, #2949 de magasin, etc.).</li></ul> | Les questions de clarification sont limitées aux composants et aux éléments de dimension. Data Insights Agent ne peut pas clarifier des éléments tels que les vues de données, les visualisations, la granularité des données, la comparaison et la portée. Lorsque des questions de clarification ne peuvent pas être utilisées, l’agent utilise par défaut ce que vous demandez le plus probablement. Si elle renvoie une visualisation ou une granularité de données inattendue, vous pouvez poser une question complémentaire ou ajuster la visualisation et les données. |
| **Vérifiabilité et exactitude des données** | La vérifiabilité et l’exactitude des données peuvent être confirmées en affichant le tableau à structure libre généré et la visualisation des données. <p>Par exemple, si vous demandez à Data Insights Agent d’*Établir la tendance des commandes le mois dernier*, vous pouvez confirmer que la mesure correcte (« commandes ») et la période (« mois dernier ») ont été sélectionnées dans le panneau, la visualisation des données et le tableau à structure libre nouvellement générés.</p> | Data Insights Agent ne répond pas en vous informant des composants ou des visualisations qui ont été ajoutés. |
| **Mécanismes de retour d’informations** | <ul><li>Pouces levés</li><li>Pouces baissés</li><li>Indicateur</li></ul> |  |


## Gérer l’accès à l’agent Data Insights {#manage-access}

<!-- markdownlint-disable MD034 -->

>[!CONTEXTUALHELP]
>id="cja-enable-data-insights-data-view"
>title="Activer pour l’agent Data Insights"
>abstract="Cette option active cette vue de données pour une utilisation avec l’agent Data Insights. L’agent Data Insights est un agent de conversation d’IA générative accessible à partir de l’assistant IA dans Customer Journey Analytics. Il vous permet d’analyser rapidement vos données à l’aide d’invites textuelles. Il crée des visualisations pertinentes dans Analysis Workspace en utilisant les composants de votre vue de données et vos données réelles."

<!-- markdownlint-enable MD034 -->

Les paramètres suivants régissent l’accès à Data Insights Agent dans Customer Journey Analytics :

* **Accès à la solution** : Data Insights Agent est disponible pour les clients éligibles pendant une durée limitée. Data Insights Agent est accessible jusqu’au 28 février 2026. Il n’est pas disponible dans Adobe Analytics.

* **Accès contractuel** : si vous ne pouvez pas utiliser Data Insights Agent dans l’assistant AI, contactez l’administrateur ou l’administratrice de votre entreprise ou l’équipe chargée du compte Adobe. Avant que votre entreprise puisse utiliser Data Insights Agent, vous devez accepter certains termes juridiques liés à l’IA générative.

* **Autorisations** : les autorisations nécessaires doivent être accordées dans le [!UICONTROL Adobe Admin Console] pour que les utilisateurs puissent accéder à Data Insights Agent.

  Pour accorder des autorisations, un [administrateur de profils de produit](https://helpx.adobe.com/fr/enterprise/using/manage-product-profiles.html) doit effectuer les étapes suivantes dans l’[!UICONTROL Admin Console] :
   1. Dans **[!UICONTROL Admin Console]**, sélectionnez l’onglet **[!UICONTROL Produits]** pour afficher la page **[!UICONTROL Tous les produits et services]**.
   1. Sélectionnez **[!UICONTROL Customer Journey Analytics]**.
   1. Dans l’onglet **[!UICONTROL Profils de produit]**, sélectionnez le titre du profil de produit pour lequel vous souhaitez fournir un accès à [!UICONTROL Assistant AI : connaissance du produit].
   1. Dans le profil de produit spécifique, sélectionnez l’onglet **[!UICONTROL Autorisations]**.

      ![Onglet Autorisations dans Admin Console](/help/agents/images/cja-agent/ai-assistant-permissions-tab.png)

   1. Dans la ligne **[!UICONTROL Outils de création de rapports]** du tableau fourni, sélectionnez l’icône de modification ![Modifier](/help/agents/images/cja-agent/Edit.svg).
   1. Faites défiler l’écran jusqu’à ou recherchez **[!UICONTROL Assistant IA : connaissance du produit]**, puis sélectionnez l’icône plus ![Ajouter un cercle](/help/agents/images/cja-agent/AddCircle.svg) en regard de cette autorisation.
   1. Faites défiler l’écran jusqu’à ou recherchez **[!UICONTROL Data Insights Agent]**, puis sélectionnez l’icône plus ![AddCircle](/help/agents/images/cja-agent/AddCircle.svg) en regard de cette autorisation.

      L’autorisation **[!UICONTROL Assistant IA : connaissance du produit]** et l’autorisation **[!UICONTROL Data Insights Agent]** sont ajoutées à la colonne **[!UICONTROL Éléments d’autorisation inclus]**.

      ![Ajouter une autorisation](/help/agents/images/cja-agent/ai-assistant-permissions.png).

   1. Sélectionnez **[!UICONTROL Enregistrer]** pour enregistrer les autorisations.

  Pour plus d’informations sur le contrôle d’accès, voir [ Contrôle d’accès ](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/access-control#access-control).

* **Accès aux vues de données** : les vues de données doivent être activées pour Data Insights Agent.

  >[!IMPORTANT]
  >
  >Tenez compte des points suivants lors de l’activation des vues de données :
  >* Vous pouvez activer un maximum de 50 vues de données par organisation IMS. Si vous activez plus de 50 vues de données pour tous les profils de produit pour une organisation donnée, le Data Insights Agent utilisera les 50 vues de données les plus utilisées.
  >  Vous pouvez utiliser les [informations de la colonne Data Insights Agent dans les vues de données](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-dataviews/manage-dataviews#manage-data-views) pour afficher le nombre de vues de données activées pour Data Insights Agent dans votre organisation IMS.
  >* Le Data Insights Agent peut référencer les vues de données incluses à un moment donné le jour même de leur activation.

  Pour activer les vues de données pour Data Insights Agent :

   1. Dans Customer Journey Analytics, sélectionnez **[!UICONTROL Gestion des données]** > **[!UICONTROL Vues des données]**.

   1. Sélectionnez une ou plusieurs vues de données à activer pour Data Insights Agent, puis sélectionnez **[!UICONTROL Activer pour Data Insights Agent]**.

      ![Activer les vues de données pour Data Insights Agent](/help/agents/images/cja-agent/data-view-enable-dia.png)

      Pour plus d’informations sur l’activation des vues de données pour Data Insights Agent, consultez les [paramètres d’IA pour une vue de données](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-dataviews/create-dataview#ai-settings/help/data-views/create-dataview.md#ai-settings).

  Pour afficher le nombre de vues de données activées pour Data Insights Agent dans votre organisation IMS :

   1. Dans Customer Journey Analytics, sélectionnez **[!UICONTROL Gestion des données]** > **[!UICONTROL Vues des données]**.

   1. Sélectionnez l’icône d’informations en haut de la colonne **[!UICONTROL Data Insights Agent]**.

      Icône d’informations de Data Insights Agent ![](/help/agents/images/cja-agent/data-insights-agent-tooltip.png)


## Accès à Data Insights Agent dans l’assistant d’IA

1. Accédez à [experience.adobe.com](https://experience.adobe.com/) et connectez-vous avec votre Adobe ID.

2. Sélectionnez **Customer Journey Analytics** sur la page d’accueil Experience Cloud.

3. Sélectionnez **[!UICONTROL Projet vierge]** dans la bannière en haut de la page des projets pour ouvrir un nouveau projet vierge.

4. Assurez-vous que la vue de données sélectionnée pour le panneau est une vue de données activée pour une utilisation avec Data Insights Agent, comme décrit dans la section [Gérer l’accès à Data Insights Agent dans Customer Journey Analytics](#manage-access-to-data-insights-agent-in-customer-journey-analytics).

5. Sélectionnez l’icône de conversation de l’assistant AI dans la zone supérieure droite de la page.

   Si l’icône de conversation n’apparaît pas, contactez votre administrateur pour qu’il active les fonctionnalités suivantes dans Admin Console :

   * Outils de création de rapports : **[!UICONTROL Assistant IA : Connaissance des produits]**

   * Outils De Vue De Données : **[!UICONTROL Data Insights Agent]**

   Pour plus d’informations, voir [Gérer l’accès à Data Insights Agent dans Customer Journey Analytics](#manage-access-to-data-insights-agent-in-customer-journey-analytics).

   ![Icône de l’assistant AI](/help/agents/images/cja-agent/ai-asst-icon.png)

6. Dans la boîte de dialogue **[!UICONTROL Demandez à propos de Customer Journey Analytics]** au bas de la page, posez une question sur la visualisation des données à l’aide de Data Insights Agent.

   Pour plus d’informations, consultez les exemples suivants.

### Exemple 1

Supposons, par exemple, que vous soyez intéressé par les commandes que votre entreprise a reçues en juillet.

**Invite:** Saisissez *« Tendance des commandes en juillet.«*

![invite AI](/help/agents/images/cja-agent/ai-asst-prompt1.png)

**Réponse :** Data Insights Agent collecte des informations en examinant les données de la vue de données, y compris les mesures et les composants. Cela traduit l’invite en dimensions et mesures appropriées dans la plage de données.

Comme vous pouvez le constater, il a généré automatiquement un graphique linéaire et un tableau à structure libre pour afficher les commandes pour juillet.

![Réponse à l’invite - graphique linéaire et tableau à structure libre](/help/agents/images/cja-agent/ai-asst-result.png)

### Exemple 2

Ensuite, vous devez comparer vos revenus par région.

**Invite :** dans la fenêtre d’invite, saisissez *« Afficher le chiffre d’affaires par région »*

**Réponse :** Data Insights Agent comprend intelligemment que par « région », vous voulez dire « région du client ». Il génère un graphique à barres qui présente le mieux les recettes par région :

![Graphique à barres](/help/agents/images/cja-agent/ai-asst-result2.png)

### Exemple 3

Ensuite, en plus de comprendre le chiffre d’affaires par région, vous souhaitez également afficher les données de bénéfice par région. Au lieu de répéter l’invite précédente, vous pouvez demander à Data Insights Agent de mettre à jour le tableau à structure libre et de visualisation le plus récent.

**Invite :** dans la fenêtre d’invite, saisissez *« Ajouter un bénéfice »*

**Réponse :** le graphique **[!UICONTROL Barres]** fournit toujours la réponse la plus concise, mais la mesure de profit a été ajoutée sous la forme d’une colonne dans le tableau à structure libre :

![Graphique à barres](/help/agents/images/cja-agent/ai-asst-result4.png)

### Exemple 4

Enfin, examinons les recettes par catégorie de produits.

**Invite :** dans la fenêtre d’invite, saisissez *« Proportion du chiffre d’affaires par catégorie de produits ».*

**Réponse :** encore une fois, Data Insights Agent sélectionne la visualisation la plus appropriée, dans ce cas la visualisation **[!UICONTROL en anneau]**, pour répondre à la question.

![Anneau](/help/agents/images/cja-agent/ai-asst-result3.png)

## Accès à Data Insights Agent dans toutes les applications Experience Cloud

Adobe Experience Platform Agent Orchestrator vous permet d’accéder aux fonctionnalités de Data Insights Agent dans plusieurs applications Adobe Experience Cloud, telles que Adobe Journey Optimizer et Real-Time CDP.

Agent Orchestrator interprète votre requête, détermine les agents spécialisés nécessaires et les orchestre pour fournir la réponse appropriée. Il effectue le suivi du contexte dans les interactions à plusieurs tours, de sorte que vous puissiez tirer parti naturellement des requêtes précédentes.

Pour plus d&#39;informations, voir [Adobe Experience Platform Agent Orchestrator](https://business.adobe.com/products/experience-platform/agent-orchestrator.html).

## Exemples d’invites de visualisation de données

Vous trouverez ci-dessous quelques exemples d’invites courantes et des visualisations utilisées par Data Insights Agent pour répondre à ces invites.

| Exemple d’invite | Visualisation attendue |
| --- | --- |
| Afficher les bénéfices en [mois] | Ligne<p>Demander une tendance ou une mesure au cours d’une certaine période par défaut renvoie une visualisation en lignes. |
| Tendance des commandes en [mois] | Ligne |
| Afficher le chiffre d’affaires par région en [mois] | Barre |
| Part des revenus par catégorie de produits | Anneau |
| Commandes par jour de la semaine, de janvier à mai | Barre |
| Afficher les commandes par genre, de mars à juin | Barre |
| Quel est le bénéfice entre les SKU de février à mai ? | Barre |
| Chiffre d’affaires par nom de magasin dans [Mois] | Barre |
| Quels ont été mes 10 principaux SKU par bénéfice au cours du [Mois] ? | Barre |
| Proportion d&#39;achats par mois de l&#39;année | Anneau |
| Bénéfice total en [mois] | Synthèse des chiffres<p>Demander le « total » d’une mesure sur une certaine période doit renvoyer une visualisation Synthèse des chiffres. |


## Bonnes pratiques en matière de promotion

Data Insights Agent traite le contexte fourni par chaque invite utilisateur et tente de répondre intelligemment avec la visualisation et les composants les plus appropriés dans un tableau à structure libre.

Les réponses peuvent varier en fonction des mots et expressions spécifiques utilisés dans l’invite, et de légères modifications de la langue peuvent entraîner des résultats différents.

Pour obtenir les meilleurs résultats, tenez compte des recommandations suivantes :

* **Soyez précis :** incluez des termes exacts pour réduire la réponse. Voici un exemple d’invite spécifique : « Ventes du mois dernier en Californie »

* **Utiliser des mesures, des dimensions et des segments clairs :** l’ajout de mesures spécifiques (telles que « Chiffre d’affaires »), de dimensions (telles que « nom du site web »), de segments (tels que « utilisateurs d’iPhone ») et de périodes (telles que « trois derniers mois ») permet à Data Insights Agent de se concentrer sur les données appropriées.

* **Poser des questions directes :** le fait de poser des questions directement permet à Data Insights Agent de fournir plus facilement des informations claires et pertinentes. Voici un exemple de question directe dans une invite : « Quel est le chiffre d’affaires moyen par catégorie de produits cette année ? »

Consultez le tableau ci-dessous pour obtenir des exemples de termes et d’expressions que vous pouvez utiliser dans les invites avec Data Insights Agent, ainsi que les types de réponses attendus.

Ces exemples sont conçus pour vous aider à vous familiariser avec la manière dont des mots ou des structures spécifiques peuvent influencer la sortie du Data Insights Agent, afin d’obtenir des informations plus précises et plus précieuses. Data Insights Agent utilise l’IA générative, de sorte que les visualisations ou les données sélectionnées peuvent varier légèrement entre des invites similaires.

| Résultat souhaité | Exemples de termes et d’expressions |
| --- | --- |
| Visualisation Synthèse des chiffres | <ul><li>Total</li></ul> |
| Comparer les composants | <ul><li>Comparer</li><li>VS</li><li>Contraste</li><li>Semaine par semaine</li><li>Mois par mois</li><li>Trimestre par trimestre</li><li>D&#39;une année sur l&#39;autre</li></ul> |
| Visualisation en anneau | <ul><li>Proportion</li><li>Part de</li><li>Répartition</li><li>Pourcentage</li><li>Contribution</li><li>Portion</li><li>Parties</li></ul> |
| Visualisation en ligne | <ul><li>Tendance</li><li>[Mesure] dans [Période]</li></ul> |
| Visualisation sous forme de barres | <ul><li>[Mesure] par [Dimension]</li></ul> |

<!--

## Beta testing expectations and requested feedback

After posing each question, carefully review the assistant's provided answer. It's crucial to evaluate the generated visualizations comprehensively before providing feedback. 

Consider the following when evaluating a response from Data Insights Agent: 

* Chat rail response or template: Evaluate the textual response provided. Is the response appropriate given the context of your prompt? 

* Visualization/chart: Evaluate the visualization. Is it the appropriate or expected visualization for your question, or would you have expected a different visualization?  

* Freeform table: Evaluate the freeform table. Is the freeform table data correct? Is it breaking down data where requested? Are the applied segments those that you requested or expected? 

* Error Message / Out-of-Scope: If a generic error message is given stating the question is out of scope, provide feedback on whether you think the out-of-scope message is appropriate, given your prompt. Was your prompt actually in scope? 

**For every response, give a thumbs up or thumbs down, based on the response.**

Following the thumbs up or thumbs down selection, please make a selection for the relevant multi-select feedback boxes. If you want to provide additional feedback, add notes in the open text box.

## Questions and Contact

* Send questions and feedback in the Beta Slack channel: #data-insights-agent-in-cja-beta

-->


## Bonnes pratiques de configuration

Vous trouverez ci-dessous les bonnes pratiques relatives à votre configuration Customer Journey Analytics (vue de données, mesures calculées, segments, etc.) pour vous assurer que le Data Insights Agent peut localiser les composants corrects et renvoyer des réponses plus précises sans avoir à vous demander des informations supplémentaires.

* **Équilibrez les composants dont vous avez besoin**. N’ajoutez pas tous les champs de vos jeux de données en tant que mesures ou composants de dimension à votre vue de données, en particulier ceux que vous ne prévoyez pas d’utiliser dans votre analyse. D’un autre côté, ne vous limitez pas strictement aux champs que vous prévoyez d’utiliser pour votre analyse. Une vue de données trop limitée limite la flexibilité de votre analyse et la fonctionnalité de Data Insights Agent.
* **Utilisez toujours des noms d’affichage conviviaux**. Assurez-vous que tous les champs que vous définissez dans votre vue de données, en tant que composant de mesure ou de dimension, ont un nom de composant convivial. Le processus de renommage des champs avec un nom convivial est particulièrement pertinent pour les champs des jeux de données du connecteur source Adobe Analytics. Ces champs comportent souvent des noms non identifiables et non conviviaux, comme `eVar41` ou `prop25`.
* **Utilisez des noms distinctifs**. Les noms distinctifs sont particulièrement pertinents lorsque vous utilisez le même champ en tant que mesure et composant de dimension dans votre vue de données. Ou lorsque vous utilisez un champ dans plusieurs composants du même type (par exemple, dans deux mesures différentes), chacun avec des paramètres de composant différents.
* **Utilisez une convention de nommage des composants**. Vous pouvez utiliser une convention de nommage des composants pour les regrouper. Par exemple, les mesures **[!UICONTROL Commandes | Produit]** et **[!UICONTROL Commandes | Client]** peuvent faire la distinction entre les différentes mesures de commande qui peuvent exister dans vos données.
* **Utiliser le dictionnaire de données**. Ajoutez des descriptions et d’autres données pertinentes pour les composants dans le dictionnaire de données. Actuellement, le Data Insights Agent n’utilise pas la description et les balises du dictionnaire de données, mais il pourrait en utiliser à l’avenir.
* **Utiliser des mesures calculées approuvées**. Convenez d’un processus pour n’utiliser que des mesures calculées approuvées comme composants dans votre vue de données et évitez d’utiliser des mesures calculées expérimentales.
* **Partage des segments requis**. Veillez à partager les segments et à rendre visibles les segments requis pour les invites de Data Insights Agent.
* **Normaliser les noms de composant dans les vues de données**. Si vous utilisez les mêmes champs en tant que composant dans plusieurs vues de données, veillez à utiliser un seul nom convivial et un seul identifiant pour ce composant. Un nom et un identifiant uniques permettent au Data Insights Agent de changer de vue de données sans perdre de contexte.


>[!MORELIKETHIS]
>
>[Paramètres des composants](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-dataviews/component-settings/overview)
>[Dictionnaire de données](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-components/data-dictionary/data-dictionary-overview)
>[Approuver la mesure calculée](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-components/cja-calcmetrics/cm-workflow/cm-approving)
>[Partage de segments ](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-components/segments/seg-share)
