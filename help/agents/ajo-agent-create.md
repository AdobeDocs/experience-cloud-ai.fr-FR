---
title: Présentation de la compétence Création d’agent de parcours
description: Découvrez comment utiliser la compétence Création Journey Agent pour créer des parcours marketing à l’aide d’invites de langage naturel dans Journey Optimizer.
solution: Journey Optimizer
product: journey optimizer
role: Admin,User,Developer
feature: AI Assistant
topic: Administration
level: Beginner
source-git-commit: 864002185f3745ca76180af192f616d1e5da0791
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 1%

---


# Parcours Create Agent : présentation des compétences et guide de l’utilisateur

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

« Créez un parcours qui démarre lorsqu’un utilisateur accède à l’emplacement de ma boutique. Envoyez une notification push pour souhaiter la bienvenue aux utilisateurs dans le magasin . Patientez 2 jours et vérifiez si l’utilisateur dispose d’une adresse e-mail valide. Si l’utilisateur dispose d’une adresse e-mail valide, envoyez une enquête par e-mail pour lui demander des informations sur son expérience en magasin. Si l’utilisateur ne dispose pas d’une adresse e-mail valide, envoyez une notification push pour demander l’enregistrement. »

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

