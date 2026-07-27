---
description: Le duel à pile ou face — jetons de jeu, mises et tirage vérifiable.
---

# Coinflip

Le **Coinflip** est un duel à pile ou face entre deux joueurs. Vous publiez une annonce avec une mise, quelqu'un l'accepte, et le tirage désigne le gagnant.

{% hint style="success" %}
**Le Coinflip ne touche jamais vos crédits.** Il utilise une monnaie qui lui est propre, les **jetons**, sans valeur boutique et impossible à acheter. Votre solde de crédits, vos achats et votre progression ne peuvent pas être perdus au Coinflip.
{% endhint %}

## 🎫 Les jetons

Les jetons servent **uniquement** au Coinflip.

| | |
| --- | --- |
| **Recharge quotidienne** | 25 jetons par jour |
| **Plafond de recharge** | 100 jetons |
| **S'achètent** | Non, jamais |
| **Convertibles en crédits** | Non |

`/coinflip claim` réclame votre recharge du jour.

{% hint style="info" %}
Le **plafond de 100** limite seulement la recharge : si votre portefeuille contient déjà 100 jetons ou plus, la recharge quotidienne n'est pas disponible. En revanche, vos **gains peuvent dépasser ce plafond** sans limite — c'est en gagnant que l'on constitue une réserve.
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

Les deux mises sont **mises sous séquestre** avant le tirage : personne ne peut se désister une fois le duel accepté.

{% hint style="warning" %}
Les 5 % prélevés sur le pot sont **détruits**, pas redistribués. Un duel ne crée donc jamais de jetons : à l'échelle du serveur, l'économie des jetons ne peut que diminuer. C'est ce qui empêche le Coinflip de devenir une source infinie de ressources.
{% endhint %}

## 🔍 Un tirage vérifiable

Le résultat n'est pas décidé au moment où vous le découvrez.

Avant qu'une annonce puisse être acceptée, le serveur enregistre l'**empreinte d'une graine aléatoire**. Cette empreinte est figée : elle ne peut plus changer. À la résolution du duel, la graine elle-même est révélée.

`/coinflip verifier <id>` recalcule le résultat à partir de cette graine, de l'identifiant du duel et de l'UUID de votre adversaire. Si le résultat annoncé ne correspondait pas, le calcul le montrerait.

{% hint style="success" %}
Autrement dit : ni le serveur ni votre adversaire ne peuvent influencer un tirage après coup, et vous pouvez le vérifier vous-même sans nous faire confiance.
{% endhint %}

## ⌨️ Commandes

| Commande | Effet |
| --- | --- |
| `/coinflip` | Ouvre le menu des annonces |
| `/coinflip claim` | Réclame la recharge quotidienne de jetons |
| `/coinflip create <mise> <face\|pile>` | Publie une annonce |
| `/coinflip accept <id>` | Accepte l'annonce d'un autre joueur |
| `/coinflip cancel` | Annule votre annonce et récupère votre mise |
| `/coinflip list` | Liste les annonces ouvertes |
| `/coinflip stats` | Votre portefeuille et vos statistiques |
| `/coinflip verifier <id>` | Vérifie le tirage d'un duel passé |

## 💡 Bon à savoir

- Vos jetons **ne se transforment jamais** en crédits, en XP ou en objets. Le Coinflip est un jeu à part entière, pas une source de progression.
- Une annonce oubliée vous est remboursée au bout de 30 minutes : vous ne perdez rien à en créer une puis à vous déconnecter.
- Vous ne pouvez avoir qu'une annonce ouverte à la fois, pour éviter de bloquer plusieurs mises en même temps.
