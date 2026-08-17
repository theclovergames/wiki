---
description: Construction libre sur parcelle, en créatif, sans PvP ni classement.
---

# Créatif

Pas de combat, pas de classement, pas de chronomètre. Une parcelle, des blocs, et le temps d'en faire quelque chose.

Le Créatif est le seul mode de Clover Games qui ne demande aucune compétence en PvP. Vous êtes en **mode créatif**, avec tous les blocs à disposition.

{% hint style="info" %}
**Pour y accéder :** depuis le lobby, **clic droit sur la boussole** de votre barre, puis Créatif dans le sélecteur de serveurs. Les commandes `/plot` ci-dessous ne fonctionnent qu'une fois sur le mode.
{% endhint %}

## 🧱 Votre parcelle

| | |
| --- | --- |
| **Parcelles par joueur** | 5 |
| **Taille** | 150 × 150 blocs |
| **Sol** | Herbe, à hauteur 50 |
| **Biome** | Jungle |
| **Hauteur de construction** | Jusqu'à 256 |
| **Invités par parcelle** | Jusqu'à 128 |

Les parcelles sont séparées par des routes et bordées d'un mur. Le mur change de couleur quand la parcelle est réclamée, ce qui permet de repérer d'un coup d'œil celles qui sont libres.

### Obtenir la vôtre

| Commande | Effet |
| --- | --- |
| `/plot auto` | Vous attribue automatiquement la première parcelle libre |
| `/plot claim` | Réclame la parcelle sur laquelle vous vous trouvez |
| `/plot home` | Vous ramène à votre parcelle |
| `/plot visit <joueur>` | Visite la parcelle d'un autre joueur |
| `/plot info` | Informations sur la parcelle où vous êtes |
| `/plot delete` | Supprime votre parcelle et tout ce qu'elle contient |

{% hint style="success" %}
**Réclamer une parcelle est gratuit.** Elle ne coûte aucun crédit, et vous pouvez en posséder **jusqu'à cinq**.
{% endhint %}

Une fois vos cinq parcelles occupées, il faut en libérer une avec `/plot delete` pour en réclamer une nouvelle. Pensez-y avant de lancer un gros projet : mieux vaut réserver une parcelle à vos essais plutôt que d'effacer une construction terminée.

{% hint style="danger" %}
`/plot delete` est **définitif**. Votre construction n'est pas récupérable, et le staff ne peut pas la restaurer.
{% endhint %}

## 👥 Construire à plusieurs

Deux niveaux d'accès, à ne pas confondre.

| Commande | Effet |
| --- | --- |
| `/plot trust <joueur>` | Accès complet, **même quand vous êtes hors ligne** |
| `/plot add <joueur>` | Accès uniquement **pendant que vous êtes connecté** |
| `/plot remove <joueur>` | Retire un accès |
| `/plot deny <joueur>` | Interdit à un joueur d'entrer sur votre parcelle |

{% hint style="warning" %}
Ne donnez `/plot trust` qu'à des personnes en qui vous avez réellement confiance : elles peuvent tout modifier et tout casser, y compris en votre absence. Pour construire ensemble sur une session, `/plot add` suffit.
{% endhint %}

## ⚙️ Ce qui est disponible

* **WorldEdit** est utilisable, mais **restreint à votre parcelle**. Impossible de déborder sur celle du voisin ou sur la route.
* **Aucun monstre n'apparaît**, ni naturellement ni par générateur. Vous construisez tranquille.
* Les **œufs d'apparition** et la **reproduction** d'animaux sont désactivés.
* La **fusion de parcelles** n'est pas activée : votre terrain garde sa taille.
* Vous pouvez changer le **biome** de votre parcelle avec `/plot setbiome <biome>`.

## 📜 Règles

Le [Règlement](../le-serveur/reglement.md) s'applique intégralement sur le Créatif.

Une parcelle est **visible par tous les joueurs**. Les constructions à caractère offensant, haineux ou sexuel sont donc traitées exactement comme un message de chat du même ordre, avec les mêmes sanctions.

Pour le reste, construisez ce que vous voulez.

{% hint style="info" %}
Vous tombez sur une construction problématique ? Ne la signalez pas dans le chat public : ouvrez un ticket avec le nom du propriétaire de la parcelle. Voir [Support et signalements](../le-serveur/support-et-signalements.md).
{% endhint %}

## 💡 Bon à savoir

* Vos **crédits, votre niveau et vos cosmétiques** vous suivent sur le Créatif comme partout ailleurs sur le réseau.
* Le mode créatif du Créatif **ne déborde pas** : les objets que vous y créez restent dans ce monde.
* `/plot help` liste l'ensemble des commandes disponibles en jeu, y compris celles qui ne figurent pas ici.

{% hint style="warning" %}
**Écrivez toujours `/plot` en entier.** Sur Clover Games, `/p` est le raccourci de votre **groupe** ([`/party`](../reference/commandes.md#social)), y compris sur le Créatif. Il n'ouvrira jamais les commandes de parcelle.
{% endhint %}
