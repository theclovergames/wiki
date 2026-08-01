---
description: >-
  Les crédits, la monnaie unique de Clover Games : comment les gagner et les
  dépenser.
---

# Crédits : l'économie du réseau

Clover Games utilise **une seule monnaie** : les **crédits**.

{% hint style="info" %}
Le [Coinflip](coinflip.md) fait exception : il utilise des **jetons** qui lui sont propres. Vos crédits ne peuvent jamais être misés ni perdus au Coinflip. Les jetons gagnés se convertissent en crédits, à raison de **100 jetons pour 1 crédit** et jamais dans l'autre sens.
{% endhint %}

Votre solde est **commun à tout le réseau** : les crédits gagnés dans un mode sont utilisables dans tous les autres, et consultables sur le [site](https://clovergames.fr) comme en jeu.

| Élément         | Valeur         |
| --------------- | -------------- |
| Nom             | Crédits        |
| Solde de départ | 0 crédit       |
| Portée          | Tout le réseau |

{% hint style="info" %}
**Référence de tarification : 100 crédits = 1,00 €.** Cette équivalence sert uniquement à fixer et comparer les prix de la boutique. Elle ne constitue **pas** une promesse de conversion ni de remboursement en argent réel : les crédits ne peuvent pas être échangés contre de l'argent.
{% endhint %}

## 📥 Gagner des crédits

### En jouant

| Source                          | Gain                                                                                                    |
| ------------------------------- | ------------------------------------------------------------------------------------------------------- |
| **Temps de jeu actif**          | 1 crédit toutes les 60 minutes (temps AFK exclu)                                                        |
| **Défis quotidiens**            | Jusqu'à 3 crédits par jour                                                                              |
| **Défis hebdomadaires**         | Jusqu'à 14 crédits par semaine                                                                          |
| **Votes**                       | Jusqu'à 1 465 crédits sur les 500 premiers votes. Voir [Votes et récompenses](votes-et-recompenses.md) |
| **Vote party**                  | 10 crédits pour les joueurs en ligne, tous les 20 votes collectifs                                      |
| **Classement mensuel de votes** | 500 crédits au 1er, 250 crédits aux 2e et 3e                                                            |
| **Fin de saison Practice**      | 0 à 100 crédits selon votre palier. Voir [Practice](../jouer/practice.md#recompenses-de-saison)        |
| **Coinflip**                    | 100 jetons pour 1 crédit, au maximum 10 crédits par jour. Voir [Coinflip](coinflip.md#convertir-vos-jetons-en-credits) |
| **Événements**                  | Variable, annoncé à chaque événement                                                                    |

{% hint style="warning" %}
Le temps **AFK ne compte pas**. Rester connecté sans jouer ne génère aucun crédit.
{% endhint %}

### En achetant

Des crédits peuvent être achetés sur la [boutique](https://clovergames.fr/shop). C'est ce qui finance l'hébergement et le développement du réseau.

### Allocation des grades

Si vous possédez un grade, vous recevez une allocation mensuelle automatique : 25 crédits (VIP), 65 (Prestige), 100 (Légende), 175 (Divin). Voir [Rangs et grades](rangs-et-grades.md).

## 🛒 Dépenser des crédits

| Dépense                              | Où                                      |
| ------------------------------------ | --------------------------------------- |
| Grades VIP, Prestige, Légende, Divin | [Boutique](https://clovergames.fr/shop) |
| Cosmétiques et effets visuels        | Boutique et menus en jeu                |
| Familiers et gadgets                 | Menus en jeu                            |
| Clefs de caisses                     | Récompenses de votes et de niveaux      |
| Services de confort                  | Boutique                                |

{% hint style="success" %}
**Rien de ce qui s'achète ne donne d'avantage en combat.** C'est une règle de conception : les crédits achètent de l'apparence et du confort, jamais de la puissance.
{% endhint %}

## 🔎 Consulter et transférer

| Commande                  | Effet                                        |
| ------------------------- | -------------------------------------------- |
| `/balance`                | Affiche votre solde : alias `/bal`, `/money` |
| `/balance <joueur>`       | Affiche le solde d'un autre joueur           |
| `/pay <joueur> <montant>` | Transfère des crédits à un joueur            |

{% hint style="danger" %}
Un transfert avec `/pay` est **immédiat et définitif**. Vérifiez le pseudo et le montant avant de valider : le staff ne rembourse pas une erreur de saisie, et « prêter » des crédits à un inconnu revient à les perdre.
{% endhint %}

## 🧾 Traçabilité

Chaque mouvement de crédits est enregistré dans un journal permanent avec son origine, sa référence et sa date.

Concrètement :

* une récompense ne peut pas être versée deux fois, même en cas de coupure ou de double clic ;
* un achat effectué sur le site est répercuté en jeu automatiquement ;
* une erreur de livraison peut être retrouvée et corrigée par le staff sur ticket ;
* une correction ne supprime jamais la transaction d'origine : elle ajoute une écriture compensatoire.

Pour toute anomalie de solde, voir [Support et signalements](support-et-signalements.md#probleme-dachat-ou-de-credits).
