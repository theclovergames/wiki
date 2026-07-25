---
description: Duels 1v1 et 2v2, kits, classement ELO, bots d'entraînement et replays.
---

# Practice — duels et classement

**Practice** est le mode compétitif de Clover Games : des duels courts, onze kits différents, un classement ELO par saison, des bots pour s'entraîner et un système de replay pour revoir ses combats.

Tapez `/practice` depuis le lobby pour commencer.

## ⚔️ Démarrer un duel

Tapez `/practice` pour ouvrir le menu. Vous choisissez d'affronter **un joueur** ou **un bot**.

| Format | Description |
| --- | --- |
| **1v1 classé** | Duel seul contre seul, compte pour votre ELO |
| **2v2 classé** | En équipe de deux, ELO séparé du 1v1 |
| **1v1 / 2v2 non classé** | Mêmes règles, sans effet sur l'ELO |
| **Duel privé** | Vous défiez un joueur précis avec `/duel` — jusqu'à 4v4 entre groupes |
| **Combat contre bot** | Entraînement avec `/botfight`, quatre difficultés |

En file classée, la fenêtre de recherche d'adversaire s'élargit progressivement et évite de vous remettre face au même joueur en boucle.

{% hint style="info" %}
Un groupe de deux rejoint le 2v2 comme équipe déjà formée. Un groupe de quatre qui choisit le 2v2 non classé est réparti automatiquement en deux équipes de deux, sans passer par la file publique. Dans un groupe de 2 à 8 joueurs, le chef peut lancer `/team split <kit>` pour créer deux camps équilibrés.
{% endhint %}

## 🎒 Les kits

Onze kits sont disponibles :

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

### Détails à connaître

- **En Boxing**, seuls les coups de mêlée directs comptent. Les balayages et les projectiles n'augmentent pas le score. Le profil livré autorise un coup toutes les 9 ticks environ.
- **En BuildUHC**, l'arène est restaurée à l'identique après chaque match.
- **Pendant le compte à rebours** (3, 2, 1, GO), vous ne pouvez ni bouger ni utiliser d'objet : interactions, nourriture, potions, projectiles et perles de l'End sont bloqués jusqu'au départ.

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

## 🏆 Classement ELO

Chaque combinaison **kit + format** possède son propre ELO.

| Élément | Valeur |
| --- | --- |
| ELO de départ | 1 000 |
| Matchs de placement | 10 (variations plus fortes) |
| Après placement | Variations moyennes, puis réduites à haut niveau |
| Durée d'une saison | 1 mois |
| Remise à zéro | Partielle : la moitié de votre écart à 1 000 est conservée |

### Paliers

Bronze · Silver · Gold · Platinum · Diamond · Master · GrandMaster

### Séries

Chaque victoire augmente votre série pour ce kit et ce format. Une défaite **ou une égalité** la remet à zéro. Votre série en cours et votre record sont conservés et visibles dans `/practice stats`.

{% hint style="warning" %}
Les **duels privés, les matchs entre groupes et les combats contre bots ne sont jamais classés**. C'est volontaire : cela empêche de fabriquer de l'ELO entre amis.
{% endhint %}

### Récompenses de saison

À la fin d'une saison, votre **meilleure cote** vous rapporte des crédits selon votre palier, à deux conditions :

- avoir joué au moins **25 matchs** ;
- avoir remporté au moins **10 victoires**.

Les montants vont de 0 à 100 crédits selon le palier. La récompense n'est versée qu'une fois, même en cas de coupure du serveur au mauvais moment.

## 🤖 Bots d'entraînement

`/botfight <kit> [easy|normal|hard|expert]`

Les bots servent à s'entraîner. Ils se déplacent, esquivent, se soignent, tirent à l'arc et utilisent les perles de l'End comme un joueur — avec les mêmes animations visibles.

{% hint style="info" %}
Monter la difficulté rend le bot **plus adroit**, jamais plus rapide : sa vitesse de déplacement reste celle d'un joueur à toutes les difficultés. Ce qui change, c'est sa précision, sa cadence, son taux de coups ratés et sa gestion des soins.
{% endhint %}

Les combats contre bots sont **enregistrés en replay** mais **n'alimentent jamais vos statistiques** : ni victoires, ni défaites, ni kills, ni dégâts.

Une arène accueille au maximum quatre combattants par camp. Selon le nombre de joueurs humains présents, les camps sont complétés par des bots pour atteindre l'équilibre.

## 🎬 Replays

Chaque match peut être revu. Le replay rejoue positions, équipements, animations et flèches, dans l'arène exacte du combat d'origine.

| Commande | Effet |
| --- | --- |
| `/replay list` | Bibliothèque de vos replays |
| `/replay watch <id>` | Lance un replay |
| `/replay pause` | Met en pause |
| `/replay speed <0.25–4>` | Change la vitesse de lecture |
| `/replay stop` | Arrête et vous ramène à votre position |

| Type de match | Conservation |
| --- | --- |
| Classé | 30 jours |
| Non classé, duel, bot | 7 jours |

Seuls les **participants** d'un match peuvent voir son replay.

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
| `/practice top <kit> <format>` | Classement d'un kit |
| `/practice history` | Vos 63 derniers combats |
| `/practice effect [set <id>]` | Gère vos effets de victoire |
| `/duel <joueur> <kit>` | Défie un joueur |
| `/duel accept` · `/duel deny` | Accepte ou refuse un défi |
| `/team split <kit>` | Répartit votre groupe en deux camps |
| `/botfight <kit> [difficulté]` | Combat d'entraînement contre un bot |
| `/replay list\|watch\|pause\|speed\|stop` | Gestion des replays |

{% hint style="info" %}
Pendant un match, seules certaines commandes sont autorisées. Les autres sont bloquées pour éviter les abus.
{% endhint %}
