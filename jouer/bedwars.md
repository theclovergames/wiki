---
description: Protégez votre lit, détruisez ceux des autres — quatre formats, saisons et replays.
---

# BedWars — en cours de création

{% hint style="warning" %}
**BedWars n'est pas encore ouvert.** Le mode est en développement, aux côtés de [SkyPvP](skypvp.md). Cette page décrit ce qui est en préparation ; certains réglages peuvent encore évoluer. L'ouverture sera annoncée sur le [Discord](https://dsc.clovergames.fr).
{% endhint %}

Chaque équipe défend un lit. Tant qu'il est intact, ses joueurs réapparaissent. Une fois détruit, chaque mort est définitive. La dernière équipe debout gagne.

## 🎮 Quatre formats

| Format | Équipes | Joueurs par équipe |
| --- | :---: | :---: |
| **Solo** | 8 | 1 |
| **Duo** | 8 | 2 |
| **Trio** | 4 | 3 |
| **Quad** | 4 | 4 |

Le chef de groupe inscrit toute son équipe avec `/bw play <format>`. Un groupe trop nombreux pour la taille d'équipe est refusé.

Le décompte démarre lorsque la file atteint **75 %** de sa capacité, et tombe à dix secondes une fois complète. Si des joueurs partent et que le seuil n'est plus atteint, il se suspend.

## 🗳️ Salle d'attente et votes

En attendant le départ, trois objets vous permettent de voter :

- la **carte** sur laquelle vous jouerez ;
- le **style de combat** : `1.8 classique` ou `1.21 moderne` ;
- l'**état de la partie**.

En cas d'égalité, le départage est aléatoire.

{% hint style="info" %}
Deux parties de styles différents peuvent tourner en même temps : le profil de combat est appliqué **par joueur**, pas par serveur.
{% endhint %}

## ⚔️ La partie

Le chat est **d'équipe par défaut**. Préfixez votre message par `!` pour parler à tout le match. Le tir allié est désactivé.

| Situation | Règle |
| --- | --- |
| **Réapparition** | 5 secondes, tant que votre lit existe |
| **Protection au respawn** | 3 secondes, annulée dès votre première attaque |
| **Chute provoquée** | Le dernier attaquant garde le crédit pendant 10 secondes |
| **Déconnexion** | Vos ressources tombent, votre place est réservée 2 minutes |

### Ce que vous gardez à la mort

- Votre **armure permanente** reste.
- Vos **outils perdent un palier**.
- Vos **cisailles** restent.
- Vos **épées achetées disparaissent**, l'épée en bois revient.
- Vos **ressources et consommables** disparaissent.

### Protection de la carte

Seuls les **lits ennemis** et les **blocs posés pendant le match** peuvent être cassés. Les explosions, pistons, liquides et objets spéciaux ne modifient jamais la carte d'origine.

## ⏱️ Le déroulé d'un match

| Temps | Événement |
| --- | --- |
| **6 min** | Générateurs de fer et de diamant améliorés |
| **12 min** | Générateurs d'émeraude améliorés |
| **18 min** | Dernier palier de générateurs |
| **22 min** | **Tous les lits sont détruits** |
| **25 min** | **La Tempête** |

La **Tempête** révèle les survivants, resserre la frontière et augmente progressivement les dégâts jusqu'à ce qu'un vainqueur se dégage. Aucun match ne s'éternise.

## 💎 Générateurs et boutique

Les générateurs produisent du fer, du diamant et de l'émeraude à des rythmes croissants. Les améliorations **Forge I à III** accélèrent en plus le fer de votre équipe.

Le partage de proximité couvre **1,5 bloc** et exclut un allié inactif depuis plus de 45 secondes — impossible de se faire porter en restant immobile près d'un générateur.

La boutique s'organise en deux marchands : les **objets** et les **améliorations**. La première page du marchand d'objets est votre **achat rapide personnalisé** ; les suivantes présentent le catalogue complet. Un achat refusé indique toujours sa raison exacte.

### Six créations Clover

En plus du catalogue habituel, six objets spécifiques à Clover Games :

- la **Plateforme d'urgence**
- la **Balise de rappel**
- le **Propulseur inertiel**
- le **Dôme anti-projectiles**
- la **Charge de brèche**
- le **Brouilleur**

## 🏆 Saisons et progression

Une saison dure **huit semaines**.

Votre **niveau de matchmaking est caché** et séparé par format ; votre **ligue affichée** est commune à tous les formats. Vos statistiques permanentes cumulent toutes les saisons, mais les points affichés ne concernent que la saison en cours.

À la rotation : le Top 10 est figé, les récompenses sont distribuées, les points repartent de zéro et votre niveau de matchmaking conserve la moitié de son écart à la moyenne. `/bw season` pour réclamer.

Les **étoiles BedWars** sont permanentes, avec un prestige visuel tous les 100 niveaux.

{% hint style="warning" %}
Deux situations conservent vos statistiques mais **ne rapportent ni points ni récompenses** : un match de moins de cinq minutes, et une quatrième rencontre contre les mêmes adversaires dans la même heure. C'est la protection contre les matchs arrangés.
{% endhint %}

## 🎬 Replays

Chaque match est enregistré : blocs, lits, achats, améliorations, projectiles, morts, réapparitions, objets spéciaux et Tempête.

`/bw replay` ouvre la bibliothèque. Vous disposez de la pause, des vitesses de 0,25× à 4×, de sauts de 10 et 30 secondes, d'une navigation par événement, du suivi d'un joueur et d'un filtre par équipe.

| Type | Conservation |
| --- | --- |
| Replay standard | 14 jours |
| Replay partagé | 30 jours |

Un replay peut être partagé par un **code de dix caractères**, révocable à tout moment.

## 🔒 Confidentialité

Votre profil BedWars est **public par défaut**. `/bw privacy` en masque les détails aux autres joueurs — jamais au staff.

## ⌨️ Commandes

| Commande | Effet |
| --- | --- |
| `/bedwars` ou `/bw` | Hub du mode |
| `/bw play <solo\|duo\|trio\|quad>` | Rejoint une file |
| `/bw leave` | Quitte la file ou la partie |
| `/bw rejoin` | Revient dans un match en cours après déconnexion |
| `/bw stats` | Vos statistiques |
| `/bw season` | Saison en cours et récompenses |
| `/bw history` | Vos matchs passés |
| `/bw replay` | Bibliothèque de replays |
| `/bw cosmetics` | Vos cosmétiques |
| `/bw privacy` | Visibilité de votre profil |

## 💡 Bon à savoir

- Un joueur éliminé reçoit un **sélecteur d'allié**, une **revanche rapide** et un retour au lobby.
- Un joueur extérieur au match **ne peut pas entrer comme spectateur** : les accès en direct sont réservés aux éliminés.
