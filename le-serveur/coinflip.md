---
description: "Le duel à pile ou face : jetons de jeu, mises et tirage vérifiable."
---

# Coinflip

Le **Coinflip** est un duel à pile ou face entre deux joueurs. Vous publiez une annonce avec une mise, quelqu'un l'accepte, et le tirage désigne le gagnant.

{% hint style="success" %}
**Vos crédits ne sont jamais misés.** Le Coinflip utilise une monnaie qui lui est propre, les **jetons**, impossible à acheter. Votre solde de crédits, vos achats et votre progression ne peuvent pas être perdus au Coinflip.
{% endhint %}

## 🎫 Les jetons

| | |
| --- | --- |
| **Recharge quotidienne** | 25 jetons par jour |
| **Plafond de recharge** | 100 jetons |
| **S'achètent** | Non, jamais |
| **Se convertissent en crédits** | Oui, à 100 jetons pour 1 crédit |
| **S'obtiennent avec des crédits** | Non, jamais |

`/coinflip claim` réclame votre recharge du jour.

{% hint style="info" %}
Le **plafond de 100** limite seulement la recharge : si votre portefeuille contient déjà 100 jetons ou plus, la recharge quotidienne n'est pas disponible. En revanche, vos **gains peuvent dépasser ce plafond** sans limite, c'est en gagnant que l'on constitue une réserve.
{% endhint %}

## 💱 Convertir vos jetons en crédits

Vos jetons finissent par valoir quelque chose, mais **peu**, et **dans un seul sens**.

```
/coinflip echange <jetons>
```

| Règle | Valeur |
| --- | --- |
| **Taux** | 100 jetons = 1 crédit |
| **Échange minimum** | 500 jetons, soit 5 crédits |
| **Multiples** | Le montant doit être un multiple de 100 |
| **Plafond quotidien** | 10 crédits par jour |
| **Sens inverse** | Impossible : un crédit ne redevient jamais un jeton |

Le taux prolonge l'échelle de la boutique : **100 jetons = 1 crédit = 0,01 €**. Autrement dit, une mise maximale de 100 jetons représente **un centime** de valeur boutique.

{% hint style="warning" %}
**On ne peut pas mettre d'argent dans le Coinflip.** Les jetons ne s'achètent pas, et les crédits ne se reconvertissent pas en jetons. Le seul moyen d'obtenir des jetons est la recharge quotidienne, puis de gagner ceux des autres.
{% endhint %}

Concrètement, il faut beaucoup de duels pour peser sur la boutique : un grade VIP à 499 crédits représente **49 900 jetons**. Le Coinflip est un jeu qui finit par rapporter un peu, pas un raccourci vers la boutique. Une heure de jeu vous rapporte déjà 1 crédit, sans risque.

{% hint style="info" %}
Le **plafond de 10 crédits par jour** existe parce qu'un très bon joueur récupère les jetons de tous les autres. Il borne ce qu'un seul compte peut convertir, même après une grosse série de victoires. Vos jetons ne sont pas perdus pour autant : ils restent dans votre portefeuille et vous les convertirez les jours suivants.
{% endhint %}

## 🪙 Jouer un duel

1. `/coinflip` ouvre le menu des annonces en cours.
2. Créez la vôtre en choisissant une mise et un côté, ou acceptez celle d'un autre joueur.
3. Le tirage est immédiat, et le gagnant emporte le pot.

| Règle | Valeur |
| --- | --- |
| **Mise minimale** | 10 jetons |
| **Mise maximale** | 100 jetons |
| **Annonces ouvertes** | 1 seule à la fois par joueur |
| **Expiration d'une annonce** | 30 minutes, avec remboursement automatique |
| **Prélèvement sur le pot** | 5 % |

Les deux mises sont **bloquées** dès que le duel est accepté : personne ne peut se désister avant le tirage.

{% hint style="warning" %}
Les 5 % prélevés sur le pot sont **détruits**, pas redistribués. Un duel ne crée donc jamais de jetons : à l'échelle du serveur, l'économie des jetons ne peut que diminuer. C'est ce qui empêche le Coinflip de devenir une source infinie de ressources.
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
| `/coinflip claim` | Réclame la recharge quotidienne de jetons |
| `/coinflip create <mise> <face\|pile>` | Publie une annonce |
| `/coinflip accept <id>` | Accepte l'annonce d'un autre joueur |
| `/coinflip cancel` | Annule votre annonce et récupère votre mise |
| `/coinflip echange <jetons>` | Convertit vos jetons en crédits |
| `/coinflip list` | Liste les annonces ouvertes |
| `/coinflip stats` | Votre portefeuille, vos statistiques et la valeur de vos jetons |
| `/coinflip verifier <id>` | Vérifie le tirage d'un duel passé |

## 💡 Bon à savoir

- Vos jetons ne se transforment **ni en XP ni en objets** : la seule sortie est la conversion en crédits, au taux ci-dessus.
- Une annonce oubliée vous est remboursée au bout de 30 minutes : vous ne perdez rien à en créer une puis à vous déconnecter.
- Vous ne pouvez avoir qu'une annonce ouverte à la fois, pour éviter de bloquer plusieurs mises en même temps.
- Si une conversion échoue, vos jetons vous sont rendus et le plafond du jour n'est pas entamé.
