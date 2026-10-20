---
description: "Combat libre : kits, coffres partagés à piller, primes, contrats et saisons."
---

# SkyPvP

{% hint style="warning" %}
**SkyPvP est ouvert et jouable.** Comme le reste du serveur, le mode reste en développement : certains réglages peuvent encore évoluer, et cette page suit les mises à jour. Les changements sont annoncés sur le [Discord](https://discord.gg/theclovergames), où vous pouvez aussi signaler bugs et problèmes d'équilibrage.
{% endhint %}

**SkyPvP** est un mode combat libre pour tous, persistant : pas de partie à rejoindre, pas de file d'attente. Vous équipez un kit, vous entrez en warzone, vos éliminations débloquent de nouveaux kits.

{% hint style="info" %}
**Pour y accéder :** depuis le lobby, **clic droit sur la boussole** de votre barre, puis SkyPvP dans le sélecteur de serveurs. Les commandes `/skypvp` ci-dessous ne fonctionnent qu'une fois sur le mode.
{% endhint %}

Le combat suit les règles **1.8** : pas de soupe, aucun effet passif de kit, et vos armes et armures **s'usent normalement**.

{% hint style="info" %}
SkyPvP et [PvPSoup](pvpsoup.md) partagent la même structure : séries, primes, saisons, classements, mais ni les mêmes règles de combat, ni le même déblocage des kits. Vos statistiques sont **séparées** entre les deux modes.
{% endhint %}

## 🗺️ Les deux zones

| Zone         | Ce qui s'y passe                                    |
| ------------ | --------------------------------------------------- |
| **Safezone** | Aucun combat. Vous prenez votre kit. Il peut y en avoir plusieurs sur la carte. |
| **Warzone**  | Tout le reste du monde. Combat libre.               |

À la connexion et après chaque mort, vous revenez en safezone **vie et faim restaurées**. Il faut prendre un kit pour repartir en warzone.

### Le tag de combat

Infliger ou recevoir des dégâts vous place **en combat pendant 10 secondes**. Pendant ce tag, impossible de rentrer en safezone ou de quitter le monde.

Le tag s'arrête **dès que votre dernier adversaire meurt**, et la barre d'action annonce la fin du combat. S'il vous reste un autre adversaire, le tag ne court plus que pour lui.

Une fois expiré, deux options :

* revenir physiquement dans la safezone ;
* utiliser `/skypvp spawn`, qui canalise le retour pendant **5 secondes**.

La canalisation est annulée par un mouvement, des dégâts, une téléportation ou un portail.

{% hint style="danger" %}
**Se déconnecter pendant le tag compte comme une mort.** L'élimination est attribuée à votre dernier attaquant, et votre équipement est partagé entre lui et ceux qui l'ont aidé, comme pour toute mort en combat.
{% endhint %}

### Votre inventaire n'est jamais réinitialisé

C'est le principe central du mode : **kits et butin se cumulent**.

Le kit s'ajoute à ce que vous portez déjà. Chaque pièce rejoint sa place habituelle si l'emplacement est libre, sinon ailleurs dans l'inventaire, sinon au sol. Et l'**armure que vous portez déjà n'est jamais remplacée**, y compris celle ramassée sur un joueur que vous venez de tuer.

Traverser la frontière, revenir au spawn ou vous déconnecter **ne vous coûte rien**. Seuls votre vie, votre faim et le feu sont remis à zéro.

{% hint style="warning" %}
**Deux exceptions, et seulement deux.**

Une **mort en combat** donne votre équipement à votre tueur et à ceux qui l'ont aidé, et se déconnecter pendant le tag de combat compte comme une telle mort.

**Quitter le monde** confisque votre équipement, pour qu'il n'arrive pas dans un autre mode.
{% endhint %}

### Un kit par vie

Puisque le kit s'ajoute à votre butin au lieu de le remplacer, vous n'y avez droit qu'**une fois par vie**. Sinon, recliquer le comptoir suffirait à se constituer un stock gratuit.

Le droit repart à votre réapparition après une mort en combat. Après une mort sans agresseur, vous gardez votre inventaire, et le droit reste consommé tant que vous portez un objet du kit. Et si vous vous déconnectez puis revenez, il est déduit de l'équipement que vous portez encore : se déconnecter ne redonne pas un kit gratuit.

## 🎒 Les kits

Huit kits, débloqués par vos **éliminations en SkyPvP**. Aucun ne s'achète.

{% hint style="warning" %}
**Aucun niveau ne compte ici.** Seul votre nombre d'éliminations en SkyPvP débloque les kits : arriver du lobby avec un gros temps de jeu ne vous donne aucun kit d'avance.

L'XP que vous gagnez en SkyPvP fait monter votre **niveau réseau**, comme dans les autres modes.
{% endhint %}

| Kit            | Éliminations | Équipement                                                              |
| -------------- | :----------: | ------------------------------------------------------------------------------ |
| **Soldat**     |      0       | Épée en fer, armure en fer Protection I                                        |
| **Archer**     |      0       | Épée en pierre, arc Puissance I, 24 flèches, maille Protection I               |
| **Éclaireur**  |      50      | Épée en fer, 2 potions de Vitesse I, maille Protection I                       |
| **Pêcheur**    |     100      | Épée en pierre, canne à pêche, armure en fer Protection I                      |
| **Gardien**    |     200      | Épée en pierre, armure en fer Protection II                                    |
| **Alchimiste** |     300      | Épée en pierre, 2 potions de Poison I, 2 de Lenteur I, maille Protection I     |
| **Berserker**  |     400      | Épée en diamant, maille sans protection                                        |
| **Ombre**      |     500      | Épée en pierre, 3 perles de l'End, 2 potions de Vitesse I, maille Protection I |

Tous les kits contiennent en plus **16 steaks** et **3 pommes dorées** : sauf le Gardien, qui en a 2.

Dans le menu des kits, un kit verrouillé affiche votre progression vers le nombre d'éliminations requis.

{% hint style="info" %}
Les noms de kits sont les mêmes qu'en [PvPSoup](pvpsoup.md#les-kits), mais **l'équipement diffère** : ici pas de soupe, et la durabilité compte.
{% endhint %}

### Arranger son kit

Comme en PvPSoup, vous pouvez **permuter** les emplacements de votre kit, sans rien ajouter ni retirer. Votre disposition est liée à la version du kit ; si le kit est mis à jour, l'ancienne disposition est ignorée.

## 📦 Coffres partagés

Des coffres sont disséminés en warzone. Seuls ceux **enregistrés par le staff** sont accessibles : les autres blocs de coffre ne s'ouvrent pas.

| Rareté     | Objets tirés | Rechargement          |
| ---------- | :----------: | --------------------- |
| **Commun** |    4 à 7     | toutes les 3 minutes  |
| **Rare**   |    3 à 5     | toutes les 5 minutes  |
| **Épique** |    2 à 4     | toutes les 10 minutes |

{% hint style="info" %}
**Le nombre d'objets n'est pas fixe.** Chaque rechargement le tire au sort dans la fourchette de son palier, donc deux coffres du même type ne rendent pas la même chose.
{% endhint %}

Un coffre ne s'ouvre pas : un **clic droit** verse tout son contenu dans votre inventaire, et ce qui n'y tient pas tombe à vos pieds. Le joueur qui pille le coffre reçoit le crédit « coffre pillé », qui compte pour vos contrats.

Le délai de rechargement démarre à ce **premier clic** après chaque génération, et il ne peut pas être repoussé : camper un coffre ne le bloque pas.

Visez un coffre pour voir sa rareté et son état dans votre barre d'action : prêt à être pillé, ou le temps restant avant le prochain rechargement.

{% hint style="warning" %}
Impossible de déposer quoi que ce soit dans un coffre, de le casser, de le faire exploser ou d'y brancher un entonnoir. Ce sont des points de loot, pas du stockage.
{% endhint %}

## ⚔️ Combat et mort

### Vos objets

Contrairement à PvPSoup, les objets ont leur **durabilité vanilla**, et ils peuvent être jetés et ramassés.

Dans le monde géré, sont bloqués : la pose et la destruction de blocs, le craft, la meule, la table de forge et les conteneurs ordinaires. L'enclume, elle, reste ouverte.

### Le partage du butin

Quand vous mourez en combat, votre équipement ne tombe pas au sol : il va **directement dans les inventaires** de ceux qui vous ont éliminé.

| Bénéficiaire       | Part                     |
| ------------------ | ------------------------ |
| **Le tueur**       | 75 %                     |
| **Les assistants** | 25 %, partagés entre eux |

* Le partage se fait unité par unité sur tout votre équipement, dans l'ordre de l'inventaire : sur quatre objets, trois vont au tueur et le quatrième à un assistant, à tour de rôle. Une arme ou une pièce d'armure n'est jamais coupée : elle part entière au tueur ou à un assistant.
* Sans assistant, le tueur reçoit tout. S'il n'est plus là (déconnecté, mort ou hors du monde), les assistants se partagent tout. Si plus personne n'est là, votre équipement tombe au sol, ou au spawn de la safezone après une chute dans le vide.
* Les enchantements et les noms des objets sont conservés.
* Un inventaire plein ne fait rien perdre : le surplus est déposé près du joueur, et lui seul peut le ramasser.

La même règle s'applique à une chute dans le vide pendant le tag et à une déconnexion en combat.

### Entretenir et améliorer son équipement

La safezone met à votre disposition des **enclumes** et des **tables d'enchantement**.

Puisque votre inventaire n'est jamais réinitialisé et que la durabilité compte, c'est là que se joue l'entretien de votre stuff : vous réparez ce qui est entamé et vous ajoutez des enchantements avec l'expérience que vous avez accumulée en warzone.

Inutile d'apporter du lapis-lazuli : chaque table en fournit **64**, renouvelés après chaque enchantement. Ce lapis reste dans la table, ne peut pas être récupéré et disparaît quand vous la fermez. Les offres d'enchantement et leur coût en niveaux d'expérience restent ceux de Minecraft.

{% hint style="success" %}
**C'est la vraie décision du mode.** Continuer avec une armure entamée pour allonger votre série, ou rentrer réparer et laisser le terrain aux autres. Un kit de départ entretenu sur plusieurs sessions n'a plus grand-chose à voir avec celui qu'on vous a donné.
{% endhint %}

{% hint style="warning" %}
Ces postes se trouvent **uniquement en safezone**, et vous ne pouvez poser aucun bloc en warzone : une armure qui lâche en plein combat ne se répare donc pas sur place, il faut rentrer.

Bonne nouvelle en revanche : les enclumes de la safezone **ne s'usent jamais** et ne peuvent pas casser.
{% endhint %}

### Chute et vide

Les **dégâts de chute sont actifs** et le **vide est mortel**. Dans les deux cas, si un joueur vous avait touché récemment, l'élimination lui est attribuée.

Sans agresseur, en revanche, une mort ne vous coûte rien : tomber dans le vide ou brûler hors combat vous laisse votre inventaire.

### Gains

| Action          | Gain                                                              |
| --------------- | ----------------------------------------------------------------- |
| **Élimination** | 15 XP                                                             |
| **Assistance**  | 5 XP : au moins 4 points de dégâts dans les 10 dernières secondes |

{% hint style="info" %}
**Anti-farm** : éliminer le même joueur ne rapporte plus rien pendant **300 secondes**.
{% endhint %}

### Ravitaillement après un kill

Une élimination vous rend **au plus une pomme dorée** (dans la limite du stock initial de votre kit) et, pour l'Archer, **8 flèches** jusqu'à un maximum de 24.

Rien d'autre n'est régénéré, ni armure, ni durabilité, ni steaks. Une longue série vous laisse de plus en plus fragile.

### Primes

Comme en PvPSoup, une série d'éliminations place une **prime** sur votre tête, qui revient au joueur qui y met fin. Voir [le détail du mécanisme](pvpsoup.md#les-primes).

## 📋 Contrats

Cinq contrats, récompensés en **pièces**. Voir [Pièces](../le-serveur/credits-economie.md).

| Rythme                | Objectifs                                 |
| --------------------- | ----------------------------------------- |
| **Quotidiens** (3)    | Éliminations, assistances, coffres pillés |
| **Hebdomadaires** (2) | Éliminations, primes                      |

`/skypvp contracts` pour les consulter.

## 🎉 Événements automatiques

Trois événements tournent d'eux-mêmes :

| Événement               | Effet                                                                               |
| ----------------------- | ----------------------------------------------------------------------------------- |
| **Carnage**             | Double l'XP des éliminations et des assistances                                     |
| **Ruée sur les primes** | Double l'XP versée par une prime                                                    |
| **Ravitaillement**      | Rend tous les coffres rechargeables et ajoute un tirage à leur prochaine génération |

## 🗓️ Saisons

Une saison dure **30 jours** (heure de Paris). Chaque saison a son propre classement, et vos statistiques all-time ne sont jamais remises à zéro.

Les récompenses de rang se réclament avec `/skypvp season claim`. Elles ne sont jamais versées deux fois, même après un redémarrage.

## 🏆 Classements

Trois statues forment le **podium** du top éliminations, avec la meilleure série de chaque joueur. Un clic ouvre le top 10.

`/skypvp top [métrique] [page]` donne les mêmes classements en jeu.

Deux tableaux muraux complètent le podium : **Top Morts** et **Top Temps de jeu**. Le premier se lit avec humour, le second récompense la simple présence.

## ⌨️ Commandes

| Commande                        | Effet                                          |
| ------------------------------- | ---------------------------------------------- |
| `/skypvp`                       | Menu principal : alias `/spvp`                 |
| `/skypvp spawn`                 | Retour à la safezone (5 s de canalisation)     |
| `/skypvp stats [joueur]`        | Statistiques                                   |
| `/skypvp top [métrique] [page]` | Classements                                    |
| `/skypvp contracts`             | Contrats quotidiens et hebdomadaires           |
| `/skypvp season [claim]`        | Saison en cours et réclamation des récompenses |

## 💡 Bon à savoir

* **Les groupes ne protègent pas** : ici c'est chacun pour soi, et deux membres d'un même groupe peuvent parfaitement se combattre.
* Vos statistiques SkyPvP sont **indépendantes** de celles de PvPSoup et de Practice.
* Gérez votre durabilité : une armure en fin de vie ne se répare pas en warzone.
