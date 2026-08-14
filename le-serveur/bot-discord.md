---
description: Niveaux, parrainage, boutique, candidatures, tickets et liaison de votre compte Minecraft.
---

# Le bot Discord

Le **Clover Bot** anime notre [Discord](https://discord.gg/theclovergames). Il gère votre progression, vos tickets, vos salons vocaux et le lien avec votre compte Minecraft.

Toutes ses fonctions passent par des **commandes slash** : tapez `/` dans n'importe quel salon pour les voir.

## 👋 À votre arrivée, et à votre départ

En rejoignant le Discord, vous recevez un **message privé de bienvenue**. Rien n'est publié dans un salon : personne d'autre n'est notifié de votre arrivée.

Si vous quittez le serveur un jour, le bot vous envoie un **court sondage privé**, en un clic. Neuf raisons sont proposées, de « je n'ai plus le temps de jouer » à « la boutique ou le pay-to-win », suivies d'un champ libre facultatif.

{% hint style="info" %}
**Répondre est facultatif, et ce n'est pas une tentative de vous faire revenir.** Ces réponses servent à savoir ce qui ne va pas : un mode qui déçoit, un manque de joueurs aux bonnes heures, une modération mal vécue. C'est plus utile qu'un départ silencieux.
{% endhint %}

Les réponses sont lues par l'équipe. Un membre **banni ou expulsé ne reçoit pas ce sondage** : il n'a pas choisi de partir, et le compter fausserait la lecture.

{% hint style="warning" %}
Discord n'autorise un message privé que vers quelqu'un avec qui le bot partage un serveur. Au moment de votre départ, ce n'est plus le cas : le sondage ne vous parvient que si le message de bienvenue avait déjà ouvert la conversation. Si vos messages privés étaient fermés à votre arrivée, vous ne recevrez rien.
{% endhint %}

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

La liaison se fait par un **code généré en jeu**, sans mot de passe et sans passer par le site.

1. En jeu, tapez **`/lier`**. Un code de huit caractères s'affiche, valable **10 minutes**.
2. Sur Discord, tapez **`/lier code:ABCD-EFGH`**.
3. Votre pseudo et votre rôle sont appliqués aussitôt, et le jeu vous confirme la liaison.

| Commande | Où | Effet |
| --- | --- | --- |
| `/lier` | En jeu | Affiche votre code, ou en génère un |
| `/lier annuler` | En jeu | Invalide le code en cours |
| `/lier code:XXXX` | Discord | Consomme le code et lie votre compte |
| `/delier` | Discord | Retire la liaison faite par code sur Discord |
| `/sync moi` | Discord | Resynchronise votre pseudo et votre rôle **Synchronisé** |

{% hint style="warning" %}
**`/delier` ne retire que la liaison faite par code sur Discord.** Si votre compte Minecraft est associé depuis le **site**, ou si votre Discord est simplement rattaché à votre compte Clover Games, c'est le site qui détient la liaison : dissociez-la dans [vos paramètres](https://clovergames.fr/profile/settings). En jeu, `/lier` vous indique la bonne marche à suivre selon votre cas.
{% endhint %}

{% hint style="success" %}
**Seul quelqu'un connecté en jeu sur ce compte peut voir le code.** C'est ce qui prouve que vous en êtes le propriétaire : personne ne peut lier votre compte Minecraft au sien.
{% endhint %}

Si vous avez déjà lié votre compte **sur le site**, la liaison est répercutée sur Discord en une minute environ. Voir [Le site web](le-site-web.md#lier-votre-compte-minecraft).

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

## 📨 Parrainage

Inviter quelqu'un rapporte **250 XP et 3 crédits**, plus des paliers à 5, 10, 25, 50 et 100 filleuls, jusqu'à 500 crédits.

| Commande | Effet |
| --- | --- |
| `/invites voir` | Vos invitations en attente, validées et refusées |
| `/invites classement` | Le classement des inviteurs |

{% hint style="warning" %}
**Rien n'est versé à l'arrivée.** Chaque invitation mûrit **sept jours**, puis n'est validée que si toutes ces conditions sont réunies :

* votre filleul est **toujours sur le Discord** ;
* son compte Discord avait **au moins 30 jours** quand il est arrivé ;
* il a **lié son compte Minecraft**, ou atteint le niveau 3 ;
* il n'était **jamais venu** auparavant ;
* vous n'avez pas dépassé votre plafond de **30 invitations par mois**.
{% endhint %}

`/invites voir` indique le **motif exact** de chaque refus : inutile de deviner.

{% hint style="info" %}
Ces règles ne visent pas à compliquer les choses, mais à ne récompenser que les vraies arrivées. Sans elles, créer des comptes serait plus rentable que jouer, alors que 3 crédits valent déjà trois heures de jeu actif.
{% endhint %}

Discord ne permet pas de savoir rétroactivement qui a invité qui **avant l'installation du bot**. Les totaux plus anciens sont repris en bloc comme historiques, et le détail nominatif ne commence qu'à cette date.

## 🪙 Boutique et crédits

Vous pouvez consulter la boutique et acheter depuis Discord, avec les **crédits de votre compte de jeu**.

| Commande | Effet |
| --- | --- |
| `/boutique voir` | Les articles payables en crédits |
| `/boutique solde` | Votre solde de crédits |
| `/boutique acheter <article>` | Achète l'article |

{% hint style="info" %}
Il n'existe **pas de monnaie Discord**. Le bot ne tient aucun compte : il interroge le site, qui débite, livre et trace l'achat exactement comme s'il avait été fait sur [clovergames.fr](https://clovergames.fr). Votre solde est le même partout. Voir [Crédits](credits-economie.md).
{% endhint %}

Un achat exige donc que votre compte Minecraft soit **lié**.

## 💡 Suggestions

`/suggestion` publie votre idée dans le salon dédié, où chacun vote 👍 ou 👎 d'un clic.

L'équipe tranche ensuite, et **vous êtes prévenu en message privé** de la décision, quelle qu'elle soit.

## 📝 Candidatures

Le panneau de recrutement du Discord reprend les **six postes** ouverts sur le site. Chaque poste a son formulaire : deux questions communes, votre disponibilité et vos éventuelles sanctions, puis trois questions propres au poste.

Votre pseudo Minecraft n'est pas demandé, il vient de votre liaison de compte.

Une fois le formulaire envoyé, le bot ouvre **un salon privé** entre vous, l'équipe et lui. C'est là que l'échange se poursuit, jamais en message privé. À la décision, le verdict est publié dans le salon **et** doublé en message privé, puis le salon est archivé.

{% hint style="info" %}
Une candidature qui demande un **portfolio ou des captures** passe par la [page de recrutement du site](https://clovergames.fr/recruitment) : un formulaire Discord ne permet pas d'y joindre de fichiers.
{% endhint %}

## 🏅 Vos grades en jeu

Votre rang sur le serveur Minecraft vous donne **automatiquement le rôle Discord correspondant**, dès que votre compte est lié.

La lecture se fait dans un sens seulement : le bot n'attribue jamais de grade en jeu depuis Discord. Il ne touche pas non plus aux rôles que l'équipe vous a donnés à la main.

## 🧑 Fiche joueur

`/joueur` recoupe un compte Discord et un compte Minecraft : niveau, grades en jeu, dernier vote et nombre de sanctions.

La réponse ne s'affiche **que pour vous**, jamais dans le salon.

## 📊 Statut des services

`/statut` affiche l'état du **site web** et **un bloc par serveur du réseau** (Lobby, PvPSoup, SkyPvP, Practice, Créatif et BedWars), avec le nombre de joueurs et l'adresse de chacun. Le message se met à jour tout seul, et `/statut <serveur>` cible un serveur en particulier.

C'est le premier endroit à consulter si vous n'arrivez pas à vous connecter : il distingue une panne générale d'un seul mode indisponible.

Deux salons vocaux affichent en permanence le **nombre de joueurs Minecraft en ligne** et le **nombre de membres du Discord**. Ils se rafraîchissent toutes les 6 minutes, toujours à cause de la limite de renommage de Discord.

## 🔨 Sanctions

Les sanctions prononcées sur le Discord sont conservées dans un **historique unique**, levées comprises. Une exclusion temporaire se lève toute seule à l'échéance, même si le bot a redémarré entre-temps.

{% hint style="warning" %}
Quand votre compte Minecraft est lié, une sanction Discord peut être **répercutée sur les serveurs de jeu**. Le Discord et le serveur ne sont pas deux mondes séparés : le [Règlement](reglement.md) s'applique aux deux.
{% endhint %}

Pour contester, voir [Support et signalements](support-et-signalements.md#contester-une-sanction).

## 🔒 Ce que le bot ne fait pas

Par choix, le bot **ne lit pas le contenu de vos messages**. L'autorisation correspondante est désactivée.

Concrètement, il n'existe **aucun journal des messages supprimés ou modifiés** sur ce serveur. Ce que vous écrivez n'est jamais archivé par le bot.

Ce qui est journalisé, à des fins de modération : les arrivées et départs, les changements de pseudo et de rôles, les sanctions, les connexions vocales et les modifications de salons.
