---
description: "Le duel à pile ou face : mises en pièces et tirage vérifiable."
---

# Coinflip

Le **Coinflip** est un duel à pile ou face entre deux joueurs. Vous publiez une annonce avec une mise, quelqu'un l'accepte, et le tirage désigne le gagnant.

{% hint style="warning" %}
**On mise de vraies pièces.** Le Coinflip utilise la monnaie du réseau, celle que vous gagnez en jouant. Ce que vous misez, vous pouvez le perdre. Des garde-fous existent (mise plafonnée, limite de perte quotidienne), mais le risque est réel : ne misez que ce que vous acceptez de perdre.
{% endhint %}

{% hint style="info" %}
**Votre progression, elle, n'est jamais en jeu.** L'XP, vos niveaux, vos kits et vos achats déjà livrés ne peuvent pas être misés ni perdus au Coinflip. Seules les pièces circulent.
{% endhint %}

## 🪙 Jouer un duel

1. `/coinflip` ouvre le menu des annonces en cours.
2. Créez la vôtre en choisissant une mise et un côté, ou acceptez celle d'un autre joueur.
3. Le tirage est immédiat, et le gagnant emporte le pot.

| Règle | Valeur |
| --- | --- |
| **Mise minimale** | 1 pièce |
| **Mise maximale** | 10 pièces, soit dix centimes de valeur boutique |
| **Perte maximale par jour** | 20 pièces |
| **Annonces ouvertes** | 1 seule à la fois par joueur |
| **Expiration d'une annonce** | 30 minutes, avec remboursement automatique |
| **Prélèvement sur le pot** | 5 % |

Les deux mises sont **bloquées** dès que le duel est accepté : personne ne peut se désister avant le tirage.

{% hint style="info" %}
La **limite de perte quotidienne** arrête les frais quand la journée tourne mal. Une fois atteinte, vous ne pouvez plus miser jusqu'au lendemain, même si votre solde le permettrait. Elle n'existe pas pour vous priver d'un jeu, mais pour qu'une mauvaise série ne coûte pas une semaine de jeu.
{% endhint %}

{% hint style="warning" %}
Les 5 % prélevés sur le pot sont **détruits**, pas redistribués. Un duel ne crée donc jamais de pièces : à l'échelle du serveur, le Coinflip retire plus de pièces qu'il n'en met en circulation. C'est ce qui l'empêche de devenir une source infinie de richesse.
{% endhint %}

## 🚫 Les enjeux restent minuscules, volontairement

Les pièces s'achètent en boutique, mais les plafonds du Coinflip sont fixés pour que ça ne change rien : une mise maximale de **10 pièces** représente **dix centimes** de valeur boutique, et la perte maximale d'une journée, vingt centimes.

Arriver avec un gros solde acheté ne sert donc à rien : on ne mise pas plus que les autres, on ne gagne pas plus vite, et une série de victoires ne rapproche d'aucun grade. Le Coinflip est un jeu d'appoint entre joueurs, pas un moyen de s'enrichir, ni d'y perdre quoi que ce soit d'important.

{% hint style="danger" %}
**Si vous jouez au Coinflip pour vous refaire, arrêtez.** Les 5 % prélevés font que, sur la durée, l'ensemble des joueurs y perd toujours. Une heure de jeu normal rapporte davantage, sans risque.
{% endhint %}

## 🔍 Un tirage vérifiable

Le résultat n'est pas décidé au moment où vous le découvrez.

Avant qu'une annonce puisse être acceptée, le serveur enregistre l'**empreinte d'une graine aléatoire**. Cette empreinte est figée : elle ne peut plus changer. À la résolution du duel, la graine elle-même est révélée.

`/coinflip verifier <id>` recalcule le résultat à partir de cette graine, de l'identifiant du duel et de l'UUID de votre adversaire. Si le résultat annoncé ne correspondait pas, le calcul le montrerait.

{% hint style="success" %}
Autrement dit, ni le serveur ni votre adversaire ne peuvent influencer un tirage après coup, et vous pouvez le vérifier vous-même sans nous faire confiance.
{% endhint %}

## 🎰 L'animation de tirage

Rejoindre un Coinflip ouvre un **écran de roulette**. La pièce défile sur sept cases, ralentit progressivement, s'immobilise sur le côté tiré, puis affiche le vainqueur, le gain et la part prélevée.

{% hint style="info" %}
**L'animation est purement décorative.** Votre mise est déjà bloquée et le résultat déjà scellé en base de données au moment où l'écran s'ouvre. La bande défilante est calée pour retomber exactement sur ce résultat : elle ne peut ni le choisir ni le contredire.
{% endhint %}

Quelques précisions :

* Celui qui **rejoint** un duel voit toujours l'animation, y compris depuis `/coinflip accept <id>`.
* Celui qui a **créé** l'annonce ne la voit que s'il a déjà un menu ouvert. On ne vous arrache jamais votre inventaire au milieu d'une partie : dans ce cas, vous recevez l'annonce du résultat dans le chat.
* **Fermer l'écran** en cours de route n'annule rien : le résultat s'affiche immédiatement dans le chat.

## ⌨️ Commandes

| Commande | Effet |
| --- | --- |
| `/coinflip` | Ouvre le menu des annonces |
| `/coinflip create <mise> <face\|pile>` | Publie une annonce |
| `/coinflip accept <id>` | Accepte l'annonce d'un autre joueur |
| `/coinflip cancel` | Annule votre annonce et récupère votre mise |
| `/coinflip list` | Liste les annonces ouvertes |
| `/coinflip stats` | Vos statistiques et votre bilan de gains et de pertes |
| `/coinflip verifier <id>` | Vérifie le tirage d'un duel passé |

## 💡 Bon à savoir

- Une annonce oubliée vous est remboursée au bout de 30 minutes : vous ne perdez rien à en créer une puis à vous déconnecter.
- Vous ne pouvez avoir qu'une annonce ouverte à la fois, pour éviter de bloquer plusieurs mises en même temps.
- `/coinflip stats` affiche votre bilan réel, gains **et** pertes. Regardez-le de temps en temps : c'est le meilleur rappel de ce que le jeu vous coûte ou vous rapporte.
- Le Coinflip ne donne ni XP, ni objet, ni avantage en combat. Il ne déplace que des pièces d'un joueur à un autre.
