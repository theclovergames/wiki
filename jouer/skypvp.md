---
description: "FFA PvP classique : kits, coffres partagés, primes, contrats et saisons."
---

# SkyPvP : FFA PvP

{% hint style="warning" %}
**SkyPvP n'est pas encore ouvert.** Le mode est en cours de création, aux côtés de [BedWars](bedwars.md). Cette page décrit ce qui est en préparation ; certains réglages peuvent encore évoluer. L'ouverture sera annoncée sur le [Discord](https://dsc.clovergames.fr).
{% endhint %}

**SkyPvP** est un mode combat libre pour tous, persistant : pas de partie à rejoindre, pas de file d'attente. Vous équipez un kit, vous entrez en warzone, vous montez en niveau.

C'est du **PvP classique** en profil **1.8** : pas de soupe, aucun effet passif de kit, et vos armes et armures **s'usent normalement**.

{% hint style="info" %}
SkyPvP et [PvPSoup](pvpsoup.md) partagent la même structure : progression, séries, primes, saisons, classements, mais pas les mêmes règles de combat. Vos statistiques sont **séparées** entre les deux modes.
{% endhint %}

## 🗺️ Les deux zones

| Zone         | Ce qui s'y passe                                    |
| ------------ | --------------------------------------------------- |
| **Safezone** | Aucun combat. Vous prenez votre kit. Il peut y en avoir plusieurs sur la carte. |
| **Warzone**  | Tout le reste du monde. Combat libre.               |

À la connexion et après chaque mort, vous revenez en safezone **vie et faim restaurées**. Il faut prendre un kit pour repartir en warzone.

### Le tag de combat

Infliger ou recevoir des dégâts vous place **en combat pendant 10 secondes**. Pendant ce tag, impossible de rentrer en safezone ou de quitter le monde.

Une fois expiré, deux options :

* revenir physiquement dans la safezone ;
* utiliser `/skypvp spawn`, qui canalise le retour pendant **5 secondes**.

La canalisation est annulée par un mouvement, des dégâts, une téléportation ou un portail.

{% hint style="danger" %}
**Se déconnecter pendant le tag compte comme une mort.** L'élimination est attribuée à votre dernier attaquant et **tout votre inventaire est lâché sur place**.
{% endhint %}

### Votre inventaire n'est jamais réinitialisé

C'est le principe central du mode : **kits et butin se cumulent**.

Le kit s'ajoute à ce que vous portez déjà. Chaque pièce rejoint sa place habituelle si l'emplacement est libre, sinon ailleurs dans l'inventaire, sinon au sol. Et l'**armure que vous portez déjà n'est jamais remplacée**, y compris celle ramassée sur un joueur que vous venez de tuer.

Traverser la frontière, revenir au spawn ou vous déconnecter **ne vous coûte rien**. Seuls votre vie, votre faim et le feu sont remis à zéro.

{% hint style="warning" %}
**Deux exceptions, et seulement deux.**

La **mort** lâche tout au sol pour votre tueur, et se déconnecter pendant le tag de combat compte comme une mort.

**Quitter le monde** confisque votre équipement, pour qu'il n'arrive pas dans un autre mode.
{% endhint %}

### Un kit par vie

Puisque le kit s'ajoute à votre butin au lieu de le remplacer, vous n'y avez droit qu'**une fois par vie**. Sinon, recliquer le comptoir suffirait à se constituer un stock gratuit.

Le droit repart à votre réapparition. Et si vous vous déconnectez puis revenez, il est déduit de l'équipement que vous portez encore : se déconnecter ne redonne pas un kit gratuit.

## 🎒 Les kits

Huit kits, débloqués par votre **niveau SkyPvP**. Aucun ne s'achète.

{% hint style="warning" %}
**Ce n'est pas votre niveau réseau qui compte ici.** SkyPvP possède sa **propre progression**, alimentée uniquement par ce que vous gagnez dans ce mode. Arriver du lobby avec un gros temps de jeu ne vous donne aucun kit d'avance.

En contrepartie, cette progression monte **plus vite** que le niveau réseau.
{% endhint %}

| Kit            | Niveau SkyPvP | Équipement                                                              |
| -------------- | :----: | ------------------------------------------------------------------------------ |
| **Soldat**     |    0   | Épée en fer, armure en fer Protection I                                        |
| **Archer**     |    0   | Épée en pierre, arc Puissance I, 24 flèches, maille Protection I               |
| **Éclaireur**  |    5   | Épée en fer, 2 potions de Vitesse I, maille Protection I                       |
| **Pêcheur**    |   10   | Épée en pierre, canne à pêche, armure en fer Protection I                      |
| **Gardien**    |   20   | Épée en pierre, armure en fer Protection II                                    |
| **Alchimiste** |   30   | Épée en pierre, 2 potions de Poison I, 2 de Lenteur I, maille Protection I     |
| **Berserker**  |   40   | Épée en diamant, maille sans protection                                        |
| **Ombre**      |   50   | Épée en pierre, 3 perles de l'End, 2 potions de Vitesse I, maille Protection I |

Tous les kits contiennent en plus **16 steaks** et **3 pommes dorées** : sauf le Gardien, qui en a 2.

{% hint style="info" %}
Les noms de kits sont les mêmes qu'en [PvPSoup](pvpsoup.md#les-kits), mais **l'équipement diffère** : ici pas de soupe, et la durabilité compte.
{% endhint %}

### Arranger son kit

Comme en PvPSoup, vous pouvez **permuter** les emplacements de votre kit, sans rien ajouter ni retirer. Votre disposition est liée à la version du kit ; si le kit est mis à jour, l'ancienne disposition est ignorée.

## 📦 Coffres partagés

Des coffres sont disséminés en warzone. Seuls ceux **enregistrés par le staff** sont accessibles : les autres blocs de coffre ne s'ouvrent pas.

| Rareté     | Objets tirés | Rechargement          |
| ---------- | :----------: | --------------------- |
| **Commun** |       4      | toutes les 3 minutes  |
| **Rare**   |       3      | toutes les 5 minutes  |
| **Épique** |       2      | toutes les 10 minutes |

Le délai de rechargement démarre au **premier accès** après chaque génération, et il ne peut pas être repoussé : camper un coffre ne le bloque pas.

Le **premier joueur à retirer un objet** d'un coffre reçoit le crédit « coffre pillé », qui compte pour vos contrats.

{% hint style="warning" %}
Impossible de déposer quoi que ce soit dans un coffre, de le casser, de le faire exploser ou d'y brancher un entonnoir. Ce sont des points de loot, pas du stockage.
{% endhint %}

## ⚔️ Combat et mort

### Vos objets

Contrairement à PvPSoup, les objets ont leur **durabilité vanilla**. Ils peuvent être jetés et ramassés, et **tout est lâché à votre mort**, avec les 5 minutes habituelles avant disparition.

Dans le monde géré, sont bloqués : la pose et la destruction de blocs, le craft, la réparation et les conteneurs ordinaires.

### Chute et vide

Les **dégâts de chute sont actifs** et le **vide est mortel**. Dans les deux cas, si un joueur vous avait touché récemment, l'élimination lui est attribuée.

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

Cinq contrats, récompensés en **crédits**. Voir [Crédits](../le-serveur/credits-economie.md).

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

* **Les groupes ne protègent pas** : le mode est FFA, deux membres d'un même groupe peuvent se combattre.
* La zone affichée sur votre tableau latéral reflète toujours votre position réelle.
* Vos statistiques SkyPvP sont **indépendantes** de celles de PvPSoup et de Practice.
* Gérez votre durabilité : une armure en fin de vie ne se répare pas en warzone.
