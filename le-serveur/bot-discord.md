---
description: Niveaux, tickets, vocaux temporaires et synchronisation de votre compte Minecraft.
---

# Le bot Discord

Le **Clover Bot** anime notre [Discord](https://dsc.clovergames.fr). Il gère votre progression, vos tickets, vos salons vocaux et le lien avec votre compte Minecraft.

Toutes ses fonctions passent par des **commandes slash** : tapez `/` dans n'importe quel salon pour les voir.

## 📈 Niveaux et classement

Vous gagnez de l'expérience en participant, de deux façons :

* en **écrivant** des messages, avec une pause de 60 secondes entre deux gains pour que le spam ne rapporte rien ;
* en **restant en vocal** avec les autres.

| Commande | Effet |
| --- | --- |
| `/rank` | Votre niveau et votre progression |
| `/classement` | Le classement du serveur |

Certains niveaux débloquent des **rôles récompense**, attribués automatiquement.

{% hint style="info" %}
**Les passages de niveau vous sont annoncés en message privé**, jamais dans un salon : personne d'autre ne reçoit de notification. Si vos messages privés sont fermés, l'annonce est simplement ignorée, mais **vos rôles vous sont attribués dans tous les cas**.
{% endhint %}

## 🔄 Lier votre compte Minecraft

`/sync moi` synchronise votre identité : votre pseudo Discord prend votre pseudo Minecraft, et vous recevez le rôle **Synchronisé**.

La liaison s'appuie sur votre compte du site. Il faut donc d'abord y associer votre compte Minecraft, comme expliqué sur [Le site web](le-site-web.md#lier-votre-compte-minecraft).

{% hint style="warning" %}
Le bot ne peut pas renommer le **propriétaire du serveur** Discord. C'est une limite de Discord, pas un dysfonctionnement.
{% endhint %}

## 🎫 Tickets

Besoin d'aide, d'un signalement ou d'un problème d'achat ? Le panneau de support contient un bouton qui vous ouvre un **salon privé** avec l'équipe.

À la fermeture du ticket, la conversation est archivée sous forme de transcription. Voir [Support et signalements](support-et-signalements.md) pour savoir quoi écrire dedans.

## 🔊 Vocaux temporaires

Rejoignez le salon **« ➕ Créer ton vocal »** : le bot vous crée aussitôt un salon vocal **et** un salon texte privé, dont vous êtes propriétaire.

Les commandes `/voc` vous permettent ensuite de le verrouiller, d'en limiter le nombre de places, de le renommer ou d'en transférer la propriété.

Le salon disparaît tout seul quand il se vide.

{% hint style="info" %}
Discord limite chaque salon à **2 renommages par tranche de 10 minutes**. Si `/voc renommer` refuse votre demande, c'est cette limite, il suffit d'attendre.
{% endhint %}

## 🎉 Concours

Les concours se lancent par l'équipe et se rejoignent d'un **clic sur un bouton**, sans commande à taper.

Certains demandent un rôle ou un niveau minimum pour participer. Un concours en cours survit à un redémarrage du bot : votre participation n'est jamais perdue.

## 🔗 Invitations

| Commande | Effet |
| --- | --- |
| `/invites voir` | Le nombre de membres que vous avez invités |
| `/invites classement` | Le classement des inviteurs |

{% hint style="info" %}
Discord ne permet pas de savoir rétroactivement qui a invité qui **avant l'installation du bot**. Les totaux plus anciens sont donc repris en bloc comme historiques, et le détail nominatif ne commence qu'à partir de cette date.
{% endhint %}

## 📊 Statut des services

`/statut` affiche l'état du **site web** et du **serveur Minecraft**, dans un message qui se met à jour tout seul. C'est le premier endroit à consulter si vous n'arrivez pas à vous connecter.

Deux salons vocaux affichent en permanence le **nombre de joueurs Minecraft en ligne** et le **nombre de membres du Discord**. Ils se rafraîchissent toutes les 6 minutes, toujours à cause de la limite de renommage de Discord.

## 🔒 Ce que le bot ne fait pas

Par choix, le bot **ne lit pas le contenu de vos messages**. L'autorisation correspondante est désactivée.

Concrètement, il n'existe **aucun journal des messages supprimés ou modifiés** sur ce serveur. Ce que vous écrivez n'est jamais archivé par le bot.

Ce qui est journalisé, à des fins de modération : les arrivées et départs, les changements de pseudo et de rôles, les sanctions, les connexions vocales et les modifications de salons.

## ⚙️ Commandes réservées à l'équipe

`/config`, `/ticket setup`, `/giveaway start` et les sous-commandes d'administration sont réservées au staff. Elles n'apparaissent pas dans votre liste si vous n'y avez pas droit.
