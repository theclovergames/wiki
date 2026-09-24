---
description: Construction libre sur parcelle, en créatif, sans PvP ni classement, et pêche au spawn.
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
**Réclamer une parcelle est gratuit.** Elle ne coûte aucune pièce, et vous pouvez en posséder **jusqu'à cinq**.
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

## 🎣 La pêche au spawn

En attendant de construire, ou entre deux sessions, vous pouvez pêcher au bord de l'eau du **spawn du Créatif**. On n'y pêche pas de poissons : chaque prise réussie rapporte une récompense.

### Obtenir la canne

**Yann**, le pêcheur du spawn, vous prête sa canne. Elle ne sert qu'au spawn :

* elle ne se jette pas, ne se range pas dans un coffre et ne s'use pas ;
* elle retourne chez Yann si vous vous éloignez de plus de **40 blocs** de l'endroit où il vous l'a prêtée, ou s'il n'y a plus d'eau à moins de **10 blocs** de vous ;
* elle vous est aussi reprise quand vous quittez le spawn, vous déconnectez ou mourez.

Gardez un emplacement libre dans votre inventaire pour la recevoir.

### Ferrer la prise

1. Lancez la canne dans l'eau et attendez.
2. Quand **« Ça mord ! »** s'affiche, une barre apparaît au-dessus de votre barre d'objets, avec un curseur qui la parcourt.
3. **Cliquez** (gauche ou droit) quand le curseur est dans la **zone verte**. Vous avez 3 secondes par clic.
4. Un clic hors de la zone verte ou un temps écoulé, et la prise file.

Plus la prise est rare, plus il faut réussir de clics, plus la zone verte est étroite et plus le curseur va vite.

### Ce que l'on peut pêcher

| Rareté | Chance | Clics à réussir | Récompenses possibles |
| --- | ---: | :---: | --- |
| Commune | 70 % | 1 | 2 à 6 pièces, ou 5 à 12 XP |
| Rare | 22 % | 2 | 10 à 25 pièces, 20 à 40 XP, ou une clé commune |
| Épique | 7 % | 3 | 40 à 80 pièces, une clé rare, ou le familier **Axolotl** |
| Légendaire | 1 % | 3 | 150 à 300 pièces, ou une clé légendaire |

Si vous possédez déjà l'Axolotl, vous recevez **100 pièces** à la place. Une prise légendaire est annoncée à tout le serveur.

{% hint style="info" %}
L'XP gagnée à la pêche compte pour votre **niveau réseau**, et les clés ouvrent les caisses de cosmétiques. La pêche n'est pas encore disponible sur le lobby principal.
{% endhint %}

## 📜 Règles

Le [Règlement](../le-serveur/reglement.md) s'applique intégralement sur le Créatif.

Une parcelle est **visible par tous les joueurs**. Les constructions à caractère offensant, haineux ou sexuel sont donc traitées exactement comme un message de chat du même ordre, avec les mêmes sanctions.

Pour le reste, construisez ce que vous voulez.

{% hint style="info" %}
Vous tombez sur une construction problématique ? Ne la signalez pas dans le chat public : ouvrez un ticket avec le nom du propriétaire de la parcelle. Voir [Support et signalements](../le-serveur/support-et-signalements.md).
{% endhint %}

## 💡 Bon à savoir

* Vos **pièces, votre niveau et vos cosmétiques** vous suivent sur le Créatif comme partout ailleurs sur le réseau.
* Le mode créatif du Créatif **ne déborde pas** : les objets que vous y créez restent dans ce monde.
* `/plot help` liste l'ensemble des commandes disponibles en jeu, y compris celles qui ne figurent pas ici.

{% hint style="warning" %}
**Écrivez toujours `/plot` en entier.** Sur Clover Games, `/p` est le raccourci de votre **groupe** ([`/party`](../reference/commandes.md#social)), y compris sur le Créatif. Il n'ouvrira jamais les commandes de parcelle.
{% endhint %}
