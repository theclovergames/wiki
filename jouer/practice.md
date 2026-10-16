---
description: Duels 1v1 et 2v2, kits, prestige compétitif commun, bots d'entraînement et replays.
---

# Practice

**Practice** est le mode compétitif de Clover Games : des duels courts, un kit pour chaque style de combat, un prestige compétitif commun à tous les kits, des bots pour s'entraîner et un système de replay pour revoir ses combats.

{% hint style="info" %}
**Pour y accéder :** depuis le lobby, **clic droit sur la boussole** de votre barre, puis Practice dans le sélecteur de serveurs. Les commandes `/practice` ci-dessous ne fonctionnent qu'une fois sur le mode.
{% endhint %}

## ⚔️ Démarrer un duel

Tapez `/practice` pour ouvrir le menu. Vous choisissez d'affronter **un joueur** ou **un bot**.

| Format | Description |
| --- | --- |
| **1v1 classé** | Duel seul contre seul, compte pour votre prestige |
| **2v2 classé** | En équipe de deux, compte pour le **même** prestige que le 1v1 |
| **1v1 / 2v2 non classé** | Mêmes règles, sans effet sur le prestige |
| **Duel privé** | Vous défiez un joueur précis avec `/duel` : jusqu'à 4v4 entre groupes |
| **Combat contre bot** | Entraînement avec `/botfight`, quatre difficultés |

En file classée, la fenêtre de recherche d'adversaire s'élargit progressivement : au bout de 15 secondes, vous pouvez tomber sur n'importe quel niveau. Les deux adversaires jouent toujours le même kit et le même format.

{% hint style="info" %}
Un groupe de deux rejoint le 2v2 comme équipe déjà formée. Un groupe de quatre qui choisit le 2v2 non classé est réparti automatiquement en deux équipes de deux, sans passer par la file publique. Dans un groupe de 2 à 8 joueurs, le chef peut lancer `/team split <kit>` pour créer deux camps équilibrés.
{% endhint %}

## 🎒 Les kits

Les kits actuellement disponibles :

| Kit | Particularité |
| --- | --- |
| `nodebuff` | Duel aux potions, sans effets négatifs |
| `debuff` | Duel aux potions, effets négatifs autorisés |
| `classic` | Duel classique |
| `vanilla` | Équipement vanilla, sans réglage particulier |
| `soup` | Soupes pour se soigner |
| `combo` | Profil de combat orienté enchaînements |
| `boxing` | **Victoire à la cible de coups**, pas aux points de vie |
| `sumo` | **Victoire en faisant tomber l'adversaire dans le vide** |
| `builduhc` | Seuls les blocs posés pendant le match peuvent être cassés |
| `archer` | Arc Puissance III, 64 flèches, armure en fer, Vitesse I |
| `axe` | Hache en netherite, bouclier et pommes dorées |

{% hint style="info" %}
`archer` et `axe` sont jouables en classé 1v1 et 2v2, mais **désactivés contre les bots** : l'IA ne reproduit pas encore fidèlement le duel d'arc ni la gestion du bouclier.
{% endhint %}

{% hint style="warning" %}
**Ce tableau n'est pas figé.** De nouveaux kits sont ajoutés au fil des mises à jour ; ils comptent tous pour le même prestige. La liste qui fait foi est celle du menu `/practice` en jeu ; si un kit y apparaît sans figurer ici, signalez-le sur le Discord.
{% endhint %}

### Détails à connaître

- **En Boxing**, seuls les coups de mêlée directs comptent. Les balayages et les projectiles n'augmentent pas le score. Le profil livré autorise un coup toutes les 9 ticks environ.
- **En BuildUHC**, l'arène est restaurée à l'identique après chaque match.
- **Pendant le compte à rebours** (3, 2, 1, GO), vous ne pouvez ni bouger ni utiliser d'objet : interactions, nourriture, potions, projectiles et perles de l'End sont bloqués jusqu'au départ.
- **Le slot que vous choisissez pendant le décompte est conservé.** Si vous vous placez sur votre épée en slot 5 avant le « GO ! », vous y êtes toujours au départ du combat. Seule la préparation initiale vous replace sur le slot 0.

## ⏳ File d'attente et inventaire

Quand vous rejoignez une file, votre inventaire est **mis de côté** et remplacé par une barre vide contenant une poudre de redstone **« Quitter la file »**.

Votre inventaire d'origine est restauré automatiquement :

- quand vous quittez la file ;
- quand le match se termine ;
- si vous vous déconnectez ou si le serveur redémarre.

{% hint style="success" %}
Vous ne pouvez pas perdre votre inventaire en jouant à Practice. Un instantané est enregistré avant chaque téléportation de match et restauré à votre reconnexion, même après un plantage.
{% endhint %}

Si aucune arène compatible n'est configurée pour le kit demandé, la file est refusée immédiatement avec un message clair.

Pendant le match, le tableau latéral affiche le **nombre d'adversaires encore en vie sur le total engagé**, sous la forme `Adversaires : 2/3`. En 2v2 comme en 4v4, c'est l'information qui compte : combien il en reste à sortir.

## 🏆 Prestige compétitif

Vous avez **un seul prestige**, commun à tous les kits et aux deux formats classés. Gagner en `nodebuff` 1v1 ou en `sumo` 2v2 fait monter le même score : changer de kit ne vous fait jamais repartir de zéro.

| Élément | Valeur |
| --- | --- |
| Score de départ | 1 000 points |
| Matchs de placement | 10, communs à tous les kits et formats (variations plus fortes) |
| Après placement | Variations moyennes, puis réduites à partir de 1 800 points |
| Durée d'une saison | 1 mois |
| Remise à zéro | Partielle : la moitié de votre écart à 1 000 est conservée |

Les points gagnés ou perdus dépendent du résultat et du niveau de l'adversaire : battre plus fort que soi rapporte davantage, perdre contre plus faible coûte davantage. À niveau égal, après le placement, une victoire rapporte environ **12 points** et une défaite en retire autant. En 2v2, c'est la moyenne de l'équipe adverse qui compte, et il n'y a aucun bonus de points par rapport au 1v1.

Pendant vos dix premiers matchs classés, votre rang s'affiche **« En placement — 4/10 »** et vous n'apparaissez pas encore au classement public. À la fin de chaque match classé, les points avant et après sont annoncés dans le chat.

### Paliers

Votre palier découle directement de vos points : il monte et redescend avec eux, et détermine votre récompense de fin de saison.

| Prestige | Points minimum | Récompense de saison |
| --- | ---: | ---: |
| **Bronze** | 0 | — |
| **Argent** | 900 | 10 pièces |
| **Or** | 1 100 | 20 pièces |
| **Platine** | 1 300 | 35 pièces |
| **Diamant** | 1 500 | 50 pièces |
| **Maître** | 1 700 | 75 pièces |
| **Grand Maître** | 1 900 | 100 pièces |

{% hint style="info" %}
Vous démarrez à 1 000 points, donc en **Prestige Argent** une fois vos placements terminés. Le même prestige s'affiche partout : menus, tableau latéral, `/practice stats` et classement.
{% endhint %}

### Adversaires déjà rencontrés

Après **trois matchs classés contre les mêmes adversaires en une heure**, vous pouvez continuer à vous affronter, mais les matchs suivants **ne modifient plus le prestige** de personne. Vous en êtes prévenus avant le départ, puis rappelés au résultat.

- Changer de kit, de format, de camp ou de partenaire ne remet pas ce compteur à zéro.
- En 2v2, il suffit qu'une paire d'adversaires ait atteint la limite pour que tout le match soit sans effet sur le prestige.
- Ces matchs restent comptés dans vos statistiques et vos replays, mais pas dans vos placements ni dans les conditions de récompense de saison.

### Séries

Chaque victoire augmente votre série pour ce kit et ce format. Une défaite **ou une égalité** la remet à zéro. Votre série en cours et votre record sont conservés et visibles dans `/practice stats`.

Le menu Statistiques affiche aussi votre **ratio victoires/défaites**, à deux décimales.

{% hint style="warning" %}
Les **duels privés, les revanches amicales, les matchs entre groupes et les combats contre bots ne sont jamais classés**. C'est volontaire : cela empêche de fabriquer du prestige entre amis. Un match annulé avant son départ ne compte pas non plus ; un abandon ou une déconnexion en plein match, en revanche, compte comme une défaite.
{% endhint %}

### Récompenses de saison

À la fin d'une saison, le **meilleur score** que vous avez atteint vous rapporte les pièces du palier correspondant. Voir le tableau ci-dessus. Deux conditions :

- avoir joué au moins **25 matchs classés** ayant compté pour le prestige ;
- avoir remporté au moins **10 de ces matchs**.

La récompense n'est versée qu'une fois, même en cas de coupure du serveur au mauvais moment.

## 📈 L'XP des duels

Chaque duel terminé rapporte de l'XP, versée à la fois sur la **progression Practice** et sur votre **niveau réseau**. Les duels privés et les matchs entre groupes en rapportent aussi, alors qu'ils ne comptent pas pour le prestige. Une défaite classée vous fait perdre des points de prestige, jamais de l'XP.

| Situation           |  XP |
| ------------------- | --: |
| Duel joué           |  20 |
| Duel gagné          |  40 |
| Duel contre un bot  |   0 |

{% hint style="info" %}
Le barème est celui de BedWars : 20 points de participation, 20 de plus pour la victoire. Un duel durant bien moins longtemps qu'une partie BedWars, l'XP à la minute y est nettement plus élevée.
{% endhint %}

Les **bots ne rapportent rien**, volontairement : ils se relancent à volonté et se gagnent sans adversaire réel.

## 🤖 Bots d'entraînement

`/botfight <kit> [easy|normal|hard|expert]`

Les bots servent à s'entraîner. Ils se déplacent, esquivent, se soignent, tirent à l'arc et utilisent les perles de l'End comme un joueur : avec les mêmes animations visibles.

{% hint style="info" %}
Monter la difficulté rend le bot **plus adroit**, jamais plus rapide : sa vitesse de déplacement reste celle d'un joueur à toutes les difficultés. Ce qui change, c'est sa précision, sa cadence, son taux de coups ratés et sa gestion des soins.
{% endhint %}

Les combats contre bots sont **enregistrés en replay** mais **n'alimentent jamais vos statistiques**, ni victoires, ni défaites, ni kills, ni dégâts.

Une arène accueille au maximum quatre combattants par camp. Selon le nombre de joueurs humains présents, les camps sont complétés par des bots pour atteindre l'équilibre.

## 🎬 Replays

Chaque match peut être revu. Le replay rejoue positions, équipements, animations et flèches, dans l'arène exacte du combat d'origine.

| Commande | Effet |
| --- | --- |
| `/replays` | Toutes vos parties, Practice et BedWars réunis |
| `/replay list` | Vos replays Practice uniquement |
| `/replay watch <id>` | Lance un replay |
| `/replay pause` | Met en pause |
| `/replay speed <0.25–4>` | Change la vitesse de lecture |
| `/replay seek <secondes>` | Avance ou recule dans le combat : `/replay seek -10` recule de 10 secondes |
| `/replay stop` | Arrête et vous ramène à votre position |

Pendant la lecture, vous volez librement autour du combat, sans pouvoir prendre de dégâts, et votre barre d'objets sert de télécommande :

- **Pause / Reprendre** ;
- **Reculer** et **Avancer** de 10 secondes, ou de 30 secondes en restant accroupi ;
- **Ralentir** et **Accélérer**, de ×0,25 à ×4 ;
- **Quitter le replay**.

Votre inventaire est mis de côté à l'ouverture et vous est rendu à la fin.

| Type de match | Conservation |
| --- | --- |
| Classé | 30 jours |
| Non classé, duel, bot | 7 jours |

Seuls les **participants** d'un match peuvent voir son replay.

## 🔁 La revanche

À la fin d'un duel 1v1 entre joueurs, les deux camps reçoivent une **offre de revanche cliquable** dans le chat.

Le **perdant** reçoit en plus un objet **Revanche** dans sa barre : un clic droit renvoie le défi au même adversaire, avec le même kit.

| | |
| --- | --- |
| **Durée de vie de l'objet** | 2 minutes |
| **Disparaît** | à la déconnexion, ou dès qu'un nouveau match démarre |
| **Non distribué** | en cas d'égalité, et après un combat contre un bot |

L'objet ne remplace jamais un objet existant de votre barre.

## 📜 Historique et revanche

`/practice history` ouvre vos **63 derniers combats** avec leur résultat.

- **Clic gauche** sur un combat : lance son replay, s'il existe encore.
- **Clic droit** après un 1v1 : propose une **revanche amicale non classée** au même adversaire, avec le même kit.

## 🎆 Effets de victoire

Un effet visuel se déclenche à la fin d'un match que vous gagnez.

| Effet | Obtention |
| --- | --- |
| **Feux d'artifice** | Gratuit, équipé par défaut |
| **Foudre** | [Boutique](https://clovergames.fr/shop), catégorie Visuels |
| **Cœurs** | Boutique, catégorie Visuels |
| **Totem** | Boutique, catégorie Visuels |

| Commande | Effet |
| --- | --- |
| `/practice effect` | Liste vos effets disponibles |
| `/practice effect set <id>` | Équipe un effet |

Votre choix est conservé d'une session à l'autre. Ces effets sont purement décoratifs.

## ⌨️ Toutes les commandes Practice

| Commande | Effet |
| --- | --- |
| `/practice` | Ouvre le menu principal |
| `/practice join <ranked\|unranked> <1v1\|2v2> <kit>` | Rejoint une file directement |
| `/practice leave` | Quitte la file ou abandonne le match |
| `/practice stats [joueur] [kit] [format]` | Statistiques détaillées |
| `/practice top` | Top 10 du prestige, tous kits et formats confondus |
| `/practice history` | Vos 63 derniers combats |
| `/practice effect [set <id>]` | Gère vos effets de victoire |
| `/duel <joueur> <kit>` | Défie un joueur. Il reçoit une invitation **cliquable** dans le chat et dispose de **30 secondes** |
| `/duel accept` · `/duel deny` | Accepte ou refuse au clavier, si les clics de chat ne fonctionnent pas chez vous |
| `/team split <kit>` | Répartit votre groupe en deux camps |
| `/botfight <kit> [difficulté]` | Combat d'entraînement contre un bot |
| `/replay list\|watch\|pause\|speed\|stop` | Gestion des replays |

{% hint style="info" %}
Pendant un match, seules certaines commandes sont autorisées. Les autres sont bloquées pour éviter les abus.
{% endhint %}
