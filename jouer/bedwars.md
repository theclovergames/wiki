---
description: "Protégez votre lit, détruisez ceux des autres : quatre formats, saisons et replays."
---

# BedWars

{% hint style="warning" %}
**BedWars est ouvert et jouable.** Comme le reste du serveur, le mode reste en développement : certains réglages peuvent encore évoluer, et cette page suit les mises à jour. Les changements sont annoncés sur le [Discord](https://discord.gg/theclovergames), où vous pouvez aussi signaler bugs et problèmes d'équilibrage.
{% endhint %}

Chaque équipe défend un lit. Tant qu'il est intact, ses joueurs réapparaissent. Une fois détruit, chaque mort est définitive. La dernière équipe debout gagne.

{% hint style="info" %}
**Pour y accéder :** depuis le lobby, **clic droit sur la boussole** de votre barre, puis BedWars dans le sélecteur de serveurs. Les commandes `/bedwars` ci-dessous ne fonctionnent qu'une fois sur le mode.
{% endhint %}

## 🎮 Quatre formats

| Format | Équipes | Joueurs par équipe |
| --- | :---: | :---: |
| **Solo** | 12 | 1 |
| **Duo** | 8 | 2 |
| **Trio** | 4 | 3 |
| **Quad** | 4 | 4 |

Le nombre d'équipes est celui des **îles de la carte** : chaque format a ses propres cartes, d'où des tailles de partie différentes.

{% hint style="info" %}
Les cartes sont regroupées par nombre d'îles avant le vote. Vous ne voterez donc jamais entre deux cartes qui n'accueillent pas le même nombre d'équipes.
{% endhint %}

Le chef de groupe inscrit toute son équipe avec `/bw play <format>`. Un groupe trop nombreux pour la taille d'équipe est refusé.

Le décompte démarre lorsque la file atteint **75 %** de sa capacité, et tombe à dix secondes une fois complète. Si des joueurs partent et que le seuil n'est plus atteint, il se suspend.

## 🗳️ Salle d'attente et votes

En attendant le départ, trois objets vous permettent de voter :

- la **carte** sur laquelle vous jouerez ;
- le **style de combat** : `1.8 classique` ou `26.2 moderne` ;
- l'**état de la partie**.

Le style voté ne s'applique qu'à votre partie : jouer en 1.8 ne demande ni serveur à part, ni version de client particulière.

En cas d'égalité, le départage est aléatoire. La **fermeture du vote** est annoncée au son, en même temps que la carte et le style retenus.

{% hint style="info" %}
**Le vote de carte est pondéré.** Un joueur possédant un grade y pèse **deux voix**, un joueur sans grade une seule ; le compteur affiché continue de compter des personnes, pas des voix. Changer d'avis déplace bien vos deux voix. Le vote du **style de combat**, lui, reste à une voix pour tout le monde.
{% endhint %}

Une poudre rouge vous permet de **quitter la file** à tout moment.

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

### Récupération : annuler ces pertes

L'amélioration d'équipe **Récupération** (4, puis 8, puis 12 diamants) retire une perte par palier :

| Palier | Ce que l'équipe cesse de perdre |
| :---: | --- |
| **I** | L'armure ne recule plus |
| **II** | Les outils non plus |
| **III** | L'épée survit, et aucune épée en bois n'est rendue par-dessus |

{% hint style="warning" %}
**Les ressources et les consommables restent perdus à tous les paliers** : pommes d'or, TNT, perles, flèches, seau d'eau. Le tueur en hérite comme avant.

C'est ce qui ramène une équipe retranchée aux générateurs. Une Récupération complète protège l'équipement, jamais les munitions.
{% endhint %}

Le palier est lu **au moment de la mort**, contrairement à Protection et Tranchant qui se posent sur l'équipement à l'achat. Améliorer pendant qu'un allié attend sa réapparition ne rattrape donc pas la mort en cours.

### Ce que rapporte une élimination

Votre tueur hérite de **la moitié de vos minerais** : fer, diamant et émeraude. Si son inventaire est plein, le surplus tombe à ses pieds.

{% hint style="success" %}
Tuer un joueur chargé de diamants vaut donc mieux que de le voir tomber dans le vide. Une mort **sans tueur**, dans le vide ou après une déconnexion, ne rend rien à personne.
{% endhint %}

### Le coffre d'équipe

Posez un **coffre de l'End** sur votre îlot : il devient le coffre partagé de votre équipe, avec 27 cases.

| Geste | Effet |
| --- | --- |
| **Clic droit** | Ouvre le coffre |
| **Clic gauche** | Y range la pile que vous tenez, sans ouvrir la grille |

Le clic gauche est le geste utile en pleine partie : déposer ses diamants en passant, sans s'arrêter devant une grille.

{% hint style="warning" %}
Le coffre d'une **équipe adverse refuse de s'ouvrir**, et son contenu ne survit pas à la fin de la partie. Ce n'est pas un rangement personnel : c'est une réserve commune, le temps d'un match.
{% endhint %}

### Les couleurs d'équipe

Le **lit** de chaque équipe prend sa couleur au lancement, et la **laine achetée** est livrée à la couleur de la vôtre.

Un pont ne dit donc plus seulement qu'il existe : il dit qui l'a tendu.

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

Ce que vous possédez déjà est **marqué d'une coche** plutôt que de vous afficher un prix : les épées, armures et paliers d'outils indiquent la raison exacte du refus, et l'icône se met à jour dès l'achat sans refermer la boutique.

### Trois objets à connaître

| Objet | Comportement |
| --- | --- |
| **Épée** | Acheter une épée **remplace** celle que vous portez. Les lames de palier inférieur sont retirées, et acheter plus faible que ce que vous tenez est refusé avant tout prélèvement |
| **TNT** | S'**amorce toute seule à la pose**, sans briquet. Environ trois secondes de mèche |
| **Seau d'eau** | L'eau se pose comme un bloc de partie : cassable, soufflée par une explosion, et vous pouvez la reprendre au seau |

{% hint style="info" %}
Vous ne pouvez pas **puiser dans l'eau de la carte**, seulement poser puis reprendre la vôtre.
{% endhint %}

Les améliorations d'équipe **Protection** et **Tranchant** suivent votre équipement neuf : une épée achetée après coup en profite, et l'épée en bois rendue à la mort la conserve.

### Les potions

Trois potions s'achètent en émeraudes. Leur couleur suffit à les reconnaître dans la barre d'objets, sans en lire le nom.

| Potion | Prix | Effet |
| --- | :---: | --- |
| **Vitesse** | 1 émeraude | Vitesse II pendant 45 secondes |
| **Saut** | 1 émeraude | Saut V pendant 45 secondes, et **plus de dégâts de chute** |
| **Invisibilité** | 2 émeraudes | 30 secondes |

{% hint style="warning" %}
**L'invisibilité ne cache pas votre armure.** Une silhouette d'armure qui traverse un pont reste parfaitement lisible : la potion sert à passer inaperçu de loin ou à rompre un combat, pas à devenir introuvable.
{% endhint %}

La potion de saut annule les dégâts de chute pendant sa durée : c'est ce qui en fait autant un outil de déplacement qu'une échappatoire.

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

Les joueurs y sont rejoués **avec leur skin d'origine**, et chaque coup encaissé est rejoué, pas seulement l'élimination finale. La boussole du lecteur ouvre la liste des joueurs de la partie, pour en suivre un directement.

L'ouverture d'un replay demande quelques secondes : une animation de chargement le signale dans la barre d'action.

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
| `/bw replay` | Vos replays BedWars uniquement |
| `/replays` | Toutes vos parties, BedWars et Practice réunis |
| `/bw cosmetics` | Vos cosmétiques |
| `/bw privacy` | Visibilité de votre profil |

## 💡 Bon à savoir

- Un joueur éliminé reçoit un **sélecteur d'allié**, une **revanche rapide** et un retour au lobby.
- Un joueur extérieur au match **ne peut pas entrer comme spectateur** : les accès en direct sont réservés aux éliminés.
