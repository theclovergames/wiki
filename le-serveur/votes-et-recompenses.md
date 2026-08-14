---
description: Voter pour Clover Games, réclamer vos paliers et suivre le classement mensuel.
---

# Votes et récompenses

Voter est **gratuit**, prend quelques secondes et aide le serveur à être visible. C'est aussi la source de crédits la plus rentable pour un joueur régulier.

## 🗳️ Comment voter

1. En jeu, tapez `/vote`.
2. Cliquez sur un site : son lien s'affiche dans le chat.
3. Cliquez le lien, votez avec votre pseudo Minecraft **exact**.
4. La récompense est comptabilisée automatiquement.

{% hint style="info" %}
Cliquer sur un site ferme votre inventaire et envoie l'adresse dans le chat : Minecraft ne permet pas à un menu d'ouvrir directement un site externe. Ce n'est pas un bug.
{% endhint %}

Vos votes sont aussi suivis sur le [Discord](bot-discord.md), qui annonce le classement du mois et attribue un rôle temporaire aux votants.

{% hint style="success" %}
**Un vote n'est jamais perdu parce que votre compte n'est pas encore lié.** Il est enregistré tel quel, et vous est crédité dès que vous liez votre compte Minecraft.
{% endhint %}

### Sites de vote

| Site |
| --- |
| Liste-Serveurs.fr |
| Serveur Minecraft Vote |
| Serveur-Minecraft.com |
| Top-Serveurs.net |

Les quatre sites sont accessibles depuis `/vote`. Chacun est comptabilisé séparément : voter sur les quatre compte pour quatre votes.

{% hint style="warning" %}
Votez avec votre **pseudo exact**, majuscules comprises. Un pseudo mal orthographié envoie le vote dans le vide et la récompense est perdue.
{% endhint %}

## 🎁 Paliers de récompenses

Vos votes s'accumulent définitivement et débloquent **21 paliers**, de 1 à 500 votes.

| Sur l'ensemble des 500 votes | Total distribué |
| --- | ---: |
| Crédits | 1 465 |
| Points d'expérience | 2 750 XP |
| Clefs de caisse *vote* | 10 |

Les paliers ne contiennent ni objet physique ni avantage de jeu : uniquement des crédits, de l'XP et des clefs cosmétiques.

{% hint style="info" %}
Les paliers ne sont **pas automatiques** : ils doivent être réclamés dans `/vote rewards`. Un palier atteint reste réclamable indéfiniment, vous ne perdez rien en tardant.
{% endhint %}

## 🎉 Vote party

Les votes de **tous les joueurs** alimentent un compteur collectif.

- Tous les **20 votes** cumulés, une *vote party* se déclenche.
- Chaque joueur **connecté à ce moment-là** reçoit 10 crédits.

La progression est visible dans `/vote`. Il n'est pas nécessaire d'avoir voté soi-même pour en profiter, mais il faut être en ligne.

## 🏆 Classement mensuel

Un classement des voteurs est tenu chaque mois et remis à zéro au changement de mois.

| Place | Récompense |
| --- | ---: |
| 1er | 100 crédits |
| 2e | 50 crédits |
| 3e | 50 crédits |

Les récompenses sont versées dès le changement de mois, ou à votre prochaine connexion si vous êtes hors ligne.

Votre total de votes depuis toujours n'est jamais réinitialisé : seul le compteur du mois repart de zéro.

## ⌨️ Commandes

| Commande | Effet |
| --- | --- |
| `/vote` | Ouvre le menu : sites, progression de la vote party, paliers, classement |
| `/vote rewards` | Réclame vos paliers débloqués |
| `/vote top` | Classement du mois en cours |
| `/vote top alltime` | Classement de tous les temps |

## ❓ Problèmes fréquents

| Situation | Cause probable |
| --- | --- |
| Mon vote n'est pas compté | Pseudo mal orthographié sur le site de vote |
| Le site dit que j'ai déjà voté | Chaque site impose un délai, généralement 24 h |
| J'ai atteint un palier mais rien reçu | Le palier doit être réclamé dans `/vote rewards` |
| Une vote party s'est déclenchée sans moi | Il faut être connecté au moment du déclenchement |

Si votre vote est bien enregistré sur le site mais absent en jeu après quelques minutes, ouvrez un ticket : voir [Support et signalements](support-et-signalements.md).
