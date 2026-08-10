---
description: "Protégez votre lit, détruisez ceux des autres : quatre formats, saisons et replays."
---

# BedWars : en cours de création

{% hint style="warning" %}
**BedWars n'est pas encore ouvert.** Le mode est en développement, aux côtés de [SkyPvP](skypvp.md). Cette page décrit ce qui est en préparation ; certains réglages peuvent encore évoluer. L'ouverture sera annoncée sur le [Discord](https://discord.gg/theclovergames).
{% endhint %}

Chaque équipe défend un lit. Tant qu'il est intact, ses joueurs réapparaissent. Une fois détruit, chaque mort est définitive. La dernière équipe debout gagne.

## 🎮 Quatre formats

Le format ne fixe qu'une chose : **le nombre de joueurs par équipe**. Le nombre d'équipes, lui, est celui des îles de la carte jouée.

| Format | Joueurs par équipe | Sur une carte à 12 îles |
| --- | :---: | :---: |
| **Solo** | 1 | 12 équipes, 12 joueurs |
| **Duo** | 2 | 12 équipes, 24 joueurs |
| **Trio** | 3 | 12 équipes, 36 joueurs |
| **Quad** | 4 | 12 équipes, 48 joueurs |

{% hint style="info" %}
Une carte plus petite accueille donc moins d'équipes, dans tous les formats. Les cartes sont regroupées par nombre d'îles avant le vote : vous ne voterez jamais entre deux cartes qui ne tiennent pas le même nombre d'équipes.
{% endhint %}

Le chef de groupe inscrit toute son équipe avec `/bw play <format>`. Un groupe trop nombreux pour la taille d'équipe est refusé.

Le décompte démarre lorsque la file atteint **75 %** de la capacité, soit 9 joueurs sur 12 en Solo, 18 sur 24 en Duo, 27 sur 36 en Trio et 36 sur 48 en Quad. Il tombe à dix secondes une fois la file complète, et se suspend si des départs repassent sous le seuil.

## 🗳️ Salle d'attente et votes

En attendant le départ, trois objets vous permettent de voter :

- la **carte** sur laquelle vous jouerez ;
- le **style de combat** : `1.8 classique` ou `1.21 moderne` ;
- l'**état de la partie**.

En cas d'égalité, le départage est aléatoire. La **fermeture du vote** est annoncée au son, en même temps que la carte et le style retenus.

Une poudre rouge vous permet de **quitter la file** à tout moment.

{% hint style="info" %}
Deux parties de styles différents peuvent tourner en même temps : le profil de combat est appliqué **par joueur**, pas par serveur.
{% endhint %}

### Choisir sa couleur d'équipe

Un **lit à la couleur de votre équipe** est posé dans la salle d'attente. Un clic dessus ouvre le choix des couleurs, avec les effectifs de chacune.

Votre placement en arène suit ce choix, et non l'équilibrage automatique. Les couleurs sont connues **avant même le vote de carte** : elles ne dépendent que du nombre d'équipes.

### Le départ

Les **cinq dernières secondes** sont annoncées en plein écran, une par une et avec un son, puis **« C'EST PARTI ! »** au lancement.

## ⚔️ La partie

Le chat est **d'équipe par défaut**. Préfixez votre message par `!` pour parler à tout le match. Le tir allié est désactivé.

{% hint style="warning" %}
**Les commandes sont verrouillées pendant une partie**, salle d'attente et vote compris. Restent autorisées : `/bw`, `/msg`, `/r`, `/party`, `/friends` et `/report`, avec leurs alias.

`/spawn` et `/tpa` sont donc refusés : ils vous sortaient de l'arène en vous laissant vivant dans la partie, lit toujours en jeu. Pour partir, utilisez `/bw leave`.
{% endhint %}

| Situation | Règle |
| --- | --- |
| **Réapparition** | 5 secondes, tant que votre lit existe |
| **Protection au respawn** | 3 secondes, annulée dès votre première attaque |
| **Chute provoquée** | Le dernier attaquant garde le crédit pendant 10 secondes |
| **Déconnexion** | Vos ressources tombent, votre place est réservée 2 minutes |

Mourir affiche un **« TU ES MORT ! »** plein écran, avec le décompte des secondes avant votre retour au spawn d'équipe. Sans lit, le titre devient **« ÉLIMINÉ »** et nomme votre tueur : vous passez spectateur.

### Ce que vous gardez à la mort

- Votre **armure recule d'un palier** : diamant → fer → mailles → cuir d'équipe, sur les quatre pièces.
- Vos **outils perdent un palier**.
- Vos **cisailles** restent.
- Vos **épées achetées disparaissent**, l'épée en bois revient.
- Vos **ressources et consommables** disparaissent.

{% hint style="info" %}
La protection payée par votre équipe est **reportée sur les pièces dégradées**. Une mort vous coûte un palier d'armure, jamais les améliorations achetées par vos coéquipiers.
{% endhint %}

### Ce que rapporte une élimination

Votre tueur hérite de **la moitié de vos minerais** : fer, diamant et émeraude. Si son inventaire est plein, le surplus tombe à ses pieds.

{% hint style="success" %}
Tuer un joueur chargé de diamants vaut donc mieux que de le voir tomber dans le vide. Une mort **sans tueur**, dans le vide ou après une déconnexion, ne rend rien à personne.
{% endhint %}

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

La **Tempête** révèle les survivants et resserre la frontière : elle s'ouvre sur **600 blocs de diamètre** et se referme sur **12 blocs en cinq minutes**, les dégâts augmentant à mesure. Aucun match ne s'éternise.

## 💎 Générateurs et boutique

Les générateurs produisent du fer, du diamant et de l'émeraude à des rythmes croissants. Les améliorations **Forge I à III** accélèrent en plus le fer de votre équipe.

Les générateurs de **diamant et d'émeraude** portent un panneau flottant : leur palier en chiffres romains, une barre de progression du cycle et le temps restant avant la prochaine production.

Le partage de proximité couvre **1,5 bloc** et exclut un allié inactif depuis plus de 45 secondes, impossible de se faire porter en restant immobile près d'un générateur.

La boutique s'organise en deux marchands : le **Marchand d'objets** et les **améliorations**. La première page du marchand est votre **achat rapide personnalisé** ; les suivantes présentent le catalogue complet. Un achat refusé indique toujours sa raison exacte.

Un même objet ne peut pas occuper deux emplacements de l'achat rapide.

### Trois objets à connaître

| Objet | Comportement |
| --- | --- |
| **Épée** | Acheter une épée **remplace** celle que vous portez. Les lames de palier inférieur sont retirées, et acheter plus faible que ce que vous tenez est refusé avant tout prélèvement |
| **TNT** | S'**amorce toute seule à la pose**, sans silex. Environ trois secondes de mèche |
| **Seau d'eau** | L'eau se pose comme un bloc de partie : cassable, soufflée par une explosion, et vous pouvez la reprendre au seau |

{% hint style="info" %}
Vous ne pouvez pas **puiser dans l'eau de la carte**, seulement poser puis reprendre la vôtre. Même règle pour la lave et la neige poudreuse.
{% endhint %}

Les améliorations d'équipe **Protection** et **Tranchant** suivent votre équipement neuf : une épée achetée après coup en profite, et l'épée en bois rendue à la mort la conserve.

### Les objets exclusifs

En plus du catalogue habituel, six objets qu'on ne trouve que sur Clover Games :

- la **Plateforme d'urgence**
- la **Balise de rappel**
- le **Propulseur inertiel**
- le **Dôme anti-projectiles**
- la **Charge de brèche**
- le **Brouilleur**

## 🪤 Les pièges d'équipe

Le menu d'améliorations permet d'armer jusqu'à **trois pièges**, coûtant 1, 2 puis 4 diamants. Ils se déclenchent **dans l'ordre de la file**, un seul à la fois.

Le premier piège de la file part dès qu'un **ennemi franchit le rayon de votre îlot**. Trois effets possibles :

| Piège | Effet |
| --- | --- |
| **Alarme** | Révèle l'intrus à toute l'équipe |
| **Fatigue du mineur** | L'assaillant ne casse plus rien correctement |
| **Cécité et lenteur** | L'assaillant avance à l'aveugle |

{% hint style="info" %}
Seule l'**entrée** dans le rayon compte, et une recharge de **30 secondes** suit chaque déclenchement. Une seule incursion ne peut donc pas vider votre file de pièges.
{% endhint %}

## 🎨 Cosmétiques

`/bw cosmetics` regroupe vos effets de victoire, de kill final et de lit détruit, ainsi que deux réglages liés à vos éliminations :

- le **son d'élimination**, joué à vous seul à chaque kill crédité ;
- le **message d'élimination**, qui remplace l'annonce générique par votre propre formule, avec le nom du tueur et de la victime aux couleurs de leurs équipes, et une variante réservée au kill final.

Comme partout sur le réseau, ces cosmétiques ne changent **rien** à la puissance de jeu.

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

Les joueurs y sont rejoués **avec leur skin d'origine**, et le tueur porte visiblement son coup à chaque élimination. L'ouverture d'un replay demande quelques secondes : une animation de chargement le signale dans la barre d'action.

| Type | Conservation |
| --- | --- |
| Replay standard | 14 jours |
| Replay partagé | 30 jours |

Un replay peut être partagé par un **code de dix caractères**, révocable à tout moment.

## 🔒 Confidentialité

Votre profil BedWars est **public par défaut**. `/bw privacy` en masque les détails aux autres joueurs, jamais au staff.

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
