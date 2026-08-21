---
description: "Combat libre et persistant : kits, safezone, primes, contrats et saisons."
---

# PvPSoup

**PvPSoup** est un mode combat libre pour tous, persistant : pas de partie à rejoindre, pas de file d'attente. Vous entrez dans la warzone, vous vous battez, vous montez en niveau et vous débloquez des kits.

Le combat utilise le profil **1.8** : enchaînements, timing de frappe et gestion des soupes.

{% hint style="info" %}
**Pour y accéder :** depuis le lobby, **clic droit sur la boussole** de votre barre, puis PvPSoup dans le sélecteur de serveurs. Les commandes `/pvpsoup` ci-dessous ne fonctionnent qu'une fois sur le mode.
{% endhint %}

## 🗺️ Les deux zones

| Zone         | Ce qui s'y passe                                             |
| ------------ | ------------------------------------------------------------ |
| **Safezone** | Aucun combat possible. Vous choisissez et équipez votre kit. |
| **Warzone**  | Tout le reste du monde. Combat libre.                        |

Pour passer en warzone, il faut **avoir équipé un kit**. Sans kit, le passage est refusé avec la raison affichée.

### Le tag de combat

Infliger ou recevoir des dégâts vous place **en combat pendant 10 secondes**.

Pendant ce tag, vous ne pouvez ni rentrer en safezone, ni quitter le monde. Une fois expiré, deux options :

* revenir physiquement dans la safezone ;
* utiliser `/pvpsoup spawn`, qui canalise le retour pendant **5 secondes**.

{% hint style="danger" %}
**Se déconnecter pendant le tag compte comme une mort**, et l'élimination est attribuée à votre dernier attaquant. Le _combat log_ ne sauve rien.
{% endhint %}

La canalisation de `/pvpsoup spawn` est annulée par un mouvement, des dégâts, une téléportation ou un portail.

## 🎒 Les kits

Huit kits, débloqués par votre **niveau PvPSoup**. **Aucun n'est plus fort qu'un autre** : ils se jouent différemment, c'est tout. Et aucun ne s'achète.

{% hint style="warning" %}
**Ce n'est pas votre niveau réseau qui compte ici.** PvPSoup possède sa **propre progression**, alimentée uniquement par ce que vous gagnez dans ce mode. Un joueur avec beaucoup de temps de jeu ailleurs sur le réseau arrive donc en warzone avec les mêmes kits que tout le monde.

La contrepartie est agréable : cette progression monte **plus vite** que le niveau réseau, puisqu'elle est plus courte.
{% endhint %}

| Kit            | Niveau PvPSoup requis |
| -------------- | :-----------: |
| **Soldat**     |       0       |
| **Archer**     |       0       |
| **Éclaireur**  |       5       |
| **Pêcheur**    |       10      |
| **Gardien**    |       20      |
| **Alchimiste** |       30      |
| **Berserker**  |       40      |
| **Ombre**      |       50      |

{% hint style="success" %}
Aucun kit ne se vend et aucun grade n'en débloque. Le seul moyen d'y accéder est de jouer.
{% endhint %}

### Choisir et arranger son kit

Le **coffre au premier emplacement** de votre barre ouvre le menu des kits.

| Action           | Effet                          |
| ---------------- | ------------------------------ |
| **Clic gauche**  | Équipe le kit                  |
| **Clic droit**   | Affiche son contenu            |
| **Shift + clic** | Ouvre l'éditeur de disposition |

Dans l'éditeur, deux clics **permutent** deux emplacements. Vous ne pouvez rien ajouter, retirer ni changer en quantité : seul l'ordre de vos objets vous appartient.

Votre disposition est liée à la version du kit. Si le kit est mis à jour, l'ancienne disposition est simplement ignorée.

## ⚔️ Combat

### Les soupes

Un **clic droit sur une soupe soigne immédiatement 7 points de vie** (3,5 cœurs), même en plein saut. La soupe disparaît entièrement : aucun bol ne reste pour encombrer votre inventaire.

{% hint style="success" %}
**Votre faim ne descend jamais** dans le monde PvPSoup. La soupe soigne, elle ne nourrit pas : vous n'avez donc aucune raison de quitter un combat pour aller manger.
{% endhint %}

### Objets de kit

Les objets fournis par votre kit sont **indroppables**, impossibles à ramasser par un autre joueur et sans durabilité. Les objets ordinaires, eux, restent manipulables normalement.

Sont bloqués pour les joueurs : les conteneurs, le craft, la réparation et la destruction de la carte.

### Gains

| Action          | Gain                                                                        |
| --------------- | --------------------------------------------------------------------------- |
| **Élimination** | 15 XP + remplissage de 5 emplacements vides avec des soupes                 |
| **Assistance**  | 5 XP : nécessite au moins 4 points de dégâts dans les 10 dernières secondes |

{% hint style="info" %}
**Anti-farm** : éliminer le même joueur ne rapporte plus rien pendant **300 secondes**. L'XP de kill, le remplissage en soupes et l'XP d'assistance sont coupés. Se tuer en boucle entre amis ne fonctionne pas.
{% endhint %}

### Les primes

À partir de **5 éliminations d'affilée**, une prime est placée sur votre tête.

Sa valeur : `20 + 5 × (série − 5)` XP, **plafonnée à 75 XP**. Elle revient au joueur qui met fin à votre série.

{% hint style="warning" %}
**La prime échappe à l'anti-farm.** Elle est toujours versée à celui qui vous arrête, même s'il vous a déjà tué récemment. En revanche, pour qu'une nouvelle prime se forme sur votre tête, il vous faut rebâtir **cinq éliminations valides** : une prime ne peut donc pas se farmer à deux.
{% endhint %}

## 📋 Contrats

Cinq contrats sont disponibles : **trois quotidiens et deux hebdomadaires**. Ils récompensent directement en **pièces**. Voir [Pièces](../le-serveur/credits-economie.md).

`/pvpsoup contracts` pour les consulter.

{% hint style="info" %}
Il n'existe **aucune monnaie propre à PvPSoup**. Tout passe par les pièces du réseau.
{% endhint %}

## 🎉 Événements automatiques

Trois événements tournent d'eux-mêmes, sans annonce préalable :

| Événement               | Effet                                            |
| ----------------------- | ------------------------------------------------ |
| **Carnage**             | Double l'XP des éliminations et des assistances  |
| **Ruée sur les primes** | Double l'XP versée par une prime                 |
| **Tempête de soupes**   | Ajoute 5 soupes au remplissage d'une élimination |

L'événement en cours s'affiche dans une **barre en haut de l'écran**, dont la jauge se vide au fil du temps : rouge pour Carnage, jaune pour Ruée sur les primes, verte pour Tempête de soupes. Elle apparaît quand vous entrez dans le monde pendant un événement et disparaît quand vous en sortez. Le chat annonce aussi le lancement et la fin.

## 🗓️ Saisons

Une saison dure **30 jours**. La **saison 1 a commencé le 1er août 2026** et se termine le 30 août au soir.

Chaque saison a son propre classement de kills. Vos statistiques all-time ne sont **jamais** remises à zéro par un changement de saison.

À la clôture, les **10 premiers** reçoivent des pièces.

| Commande                | Effet                                                                |
| ----------------------- | -------------------------------------------------------------------- |
| `/pvpsoup season`       | Période en cours, top 10, vos statistiques et vos pièces en attente |
| `/pvpsoup season claim` | Réclame vos pièces de fin de saison                                 |

{% hint style="info" %}
Les pièces de saison ne sont jamais versées deux fois, même si le serveur redémarre au mauvais moment.
{% endhint %}

## 🏆 Classements

Trois statues forment le **podium** du top kills all-time, avec les éliminations et la meilleure série de chaque joueur.

Un clic sur une statue ouvre le top 10, avec cinq onglets : **Kills**, **K/D**, **Assists**, **Meilleure série** et **Primes**.

Un panneau `Top 10` est également affiché en jeu. Les classements se rafraîchissent toutes les cinq minutes.

Deux tableaux muraux s'ajoutent au podium : **Top Morts** et **Top Temps de jeu**. Le premier se lit avec humour, le second récompense la simple présence.

## ⌨️ Commandes

| Commande                         | Effet                                          |
| -------------------------------- | ---------------------------------------------- |
| `/pvpsoup`                       | Menu principal                                 |
| `/pvpsoup spawn`                 | Retour à la safezone (5 s de canalisation)     |
| `/pvpsoup stats [joueur]`        | Vos statistiques, ou celles d'un autre joueur  |
| `/pvpsoup top [métrique] [page]` | Classements                                    |
| `/pvpsoup contracts`             | Vos contrats quotidiens et hebdomadaires       |
| `/pvpsoup season [claim]`        | Saison en cours et réclamation des récompenses |

## 💡 Bon à savoir

* **Les groupes ne protègent pas** : ici c'est chacun pour soi, et deux membres d'un même groupe peuvent parfaitement se combattre.
* La zone affichée sur votre tableau latéral reflète toujours votre position réelle, ni une téléportation ni une permission ne peut la désynchroniser.
* **Le vide ne pardonne pas en warzone.** Le filet de sécurité qui rattrape les chutes ailleurs sur le réseau est désactivé pendant un combat : tomber vous tue, sinon la chute serait une échappatoire gratuite. Une chute depuis la safezone, elle, vous rattrape toujours.
* Plusieurs safezones peuvent coexister sur la carte, et le spawn peut se trouver dans n'importe laquelle.
