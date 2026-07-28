---
description: Référence complète des commandes joueur de Clover Games.
---

# Toutes les commandes

Toutes les commandes de cette page sont accessibles à **tous les joueurs**, sauf celles marquées d'un grade. Les commandes réservées au staff ne sont pas documentées ici.

{% hint style="info" %}
Perdu ? `/help` en jeu donne l'aide contextuelle par catégories, et `/rules` rappelle le [Règlement](../le-serveur/reglement.md).
{% endhint %}

## ⭐ Essentiel

| Commande | Alias | Effet |
| --- | --- | --- |
| `/help` | `/aide` | Aide en jeu, par catégories |
| `/rules` | | Rappel du règlement |
| `/spawn` | | Retour au point de départ |
| `/back` | `/retour` | Retour à votre position précédente, ou au lieu de votre mort |
| `/afk` | | Vous signale comme absent |
| `/discord` | | Lien vers le Discord |
| `/site` | | Lien vers le site |
| `/clovermenu` | | Ouvre les menus Clover |

{% hint style="warning" %}
Le temps passé en **AFK ne rapporte aucun crédit** et suspend votre progression. Voir [Crédits](../le-serveur/credits-economie.md#gagner-des-credits).
{% endhint %}

`/back` retient vos morts et vos téléportations importantes. En revanche, cet historique **ne survit pas à un redémarrage du serveur**.

## 🏠 Homes et warps

| Commande | Effet |
| --- | --- |
| `/sethome [nom]` | Définit un point de retour personnel |
| `/home [nom]` | Vous y téléporte |
| `/homes` | Liste vos homes |
| `/delhome <nom>` | Supprime un home |
| `/warp <nom>` | Rejoint une destination du serveur |
| `/warps` | Liste les destinations disponibles |

Le nombre de homes dépend de votre grade : **1** par défaut, **3** avec VIP, **5** avec Légende. Voir [Rangs et grades](../le-serveur/rangs-et-grades.md).

## 🌀 Téléportation entre joueurs

| Commande | Effet |
| --- | --- |
| `/tpa <joueur>` | Demande à vous téléporter chez un joueur |
| `/tpahere <joueur>` | Demande à un joueur de venir chez vous |
| `/tpaccept` | Accepte une demande reçue |
| `/tpdeny` | Refuse une demande reçue |
| `/tptoggle` | Bloque ou débloque les demandes entrantes |

## 💬 Communication

| Commande | Effet |
| --- | --- |
| `/msg <joueur> <message>` | Message privé |
| `/r <message>` | Répond au dernier message privé reçu |
| `/ignore <joueur>` | Ignore un joueur |
| `/chathistory` | Consulte l'historique du chat |

## 👥 Social

| Commande | Alias | Effet |
| --- | --- | --- |
| `/friends` | | Gère vos amis et voit qui est en ligne |
| `/party` | `/p` | Gère votre groupe, entre les serveurs |
| `/visibility` | | Choisit qui vous voyez : tout le monde, vos amis et votre groupe, ou personne |

## 💰 Économie

| Commande | Alias | Effet |
| --- | --- | --- |
| `/balance` | `/bal`, `/money` | Votre solde de crédits |
| `/balance <joueur>` | | Solde d'un autre joueur |
| `/pay <joueur> <montant>` | | Transfère des crédits |
| `/shop` | | Ouvre la boutique en jeu |

{% hint style="danger" %}
`/pay` est immédiat et définitif. Vérifiez le pseudo et le montant.
{% endhint %}

## 🪙 Coinflip

Le Coinflip utilise des **jetons**, jamais vos crédits.

| Commande | Effet |
| --- | --- |
| `/coinflip` | Menu des annonces |
| `/coinflip claim` | Recharge quotidienne de 25 jetons |
| `/coinflip create <mise> <face\|pile>` | Publie une annonce |
| `/coinflip accept <id>` | Accepte une annonce |
| `/coinflip cancel` | Annule votre annonce |
| `/coinflip list` | Annonces ouvertes |
| `/coinflip stats` | Portefeuille et statistiques |
| `/coinflip verifier <id>` | Vérifie le tirage d'un duel passé |

Tous les détails sont sur [Coinflip](../le-serveur/coinflip.md).

## 📈 Progression

| Commande | Alias | Effet |
| --- | --- | --- |
| `/leveling` | | Vos niveaux, votre XP et vos récompenses |
| `/challenges` | | Défis quotidiens et hebdomadaires |
| `/playtime` | `/tempsdejeu` | Votre temps de jeu et vos paliers |
| `/vote` | | Sites de vote, paliers et classement |
| `/vote rewards` | | Réclame vos paliers de vote |
| `/vote top [alltime]` | | Classement mensuel ou général |

## 🎨 Personnalisation

| Commande | Effet |
| --- | --- |
| `/pets` | Vos familiers |
| `/gadget` | Vos cosmétiques et gadgets |
| `/doublejump` | Active ou désactive votre double saut |
| `/scoreboard` | Affiche ou masque le tableau latéral |

## 🍲 PvPSoup

| Commande | Effet |
| --- | --- |
| `/pvpsoup` | Menu principal du mode |
| `/pvpsoup spawn` | Retour à la safezone (5 s de canalisation) |
| `/pvpsoup stats [joueur]` | Statistiques |
| `/pvpsoup top [métrique] [page]` | Classements |
| `/pvpsoup contracts` | Contrats quotidiens et hebdomadaires |
| `/pvpsoup season [claim]` | Saison en cours et récompenses |

Tous les détails sont sur [PvPSoup](../jouer/pvpsoup.md).

## ☁️ SkyPvP

{% hint style="info" %}
Mode **en cours de création**, pas encore accessible. Voir [SkyPvP](../jouer/skypvp.md).
{% endhint %}

| Commande | Alias | Effet |
| --- | --- | --- |
| `/skypvp` | `/spvp` | Menu principal du mode |
| `/skypvp spawn` | | Retour à la safezone (5 s de canalisation) |
| `/skypvp stats [joueur]` | | Statistiques |
| `/skypvp top [métrique] [page]` | | Classements |
| `/skypvp contracts` | | Contrats quotidiens et hebdomadaires |
| `/skypvp season [claim]` | | Saison en cours et récompenses |

## 🛏️ BedWars

{% hint style="info" %}
Mode **en cours de création**, pas encore accessible. Voir [BedWars](../jouer/bedwars.md).
{% endhint %}

| Commande | Effet |
| --- | --- |
| `/bedwars` ou `/bw` | Hub du mode |
| `/bw play <solo\|duo\|trio\|quad>` | Rejoint une file |
| `/bw leave` · `/bw rejoin` | Quitte ou revient dans un match |
| `/bw stats` · `/bw history` | Statistiques et matchs passés |
| `/bw season` | Saison et récompenses |
| `/bw replay` | Bibliothèque de replays |
| `/bw cosmetics` · `/bw privacy` | Cosmétiques et visibilité du profil |

## ⚔️ Practice

| Commande | Effet |
| --- | --- |
| `/practice` | Menu du mode Practice |
| `/practice join <ranked\|unranked> <1v1\|2v2> <kit>` | Rejoint une file |
| `/practice leave` | Quitte la file ou abandonne |
| `/practice stats [joueur] [kit] [format]` | Statistiques |
| `/practice top <kit> <format>` | Classement d'un kit |
| `/practice history` | Vos 63 derniers combats |
| `/practice effect [set <id>]` | Effets de victoire |
| `/duel <joueur> <kit>` | Défie un joueur, invitation cliquable valable 30 s |
| `/duel accept` · `/duel deny` | Répond à un défi au clavier |
| `/team split <kit>` | Répartit votre groupe en deux camps |
| `/botfight <kit> [easy\|normal\|hard\|expert]` | Entraînement contre un bot |
| `/replay list` | Vos replays |
| `/replay watch <id>` | Lance un replay |
| `/replay pause` · `/replay stop` | Contrôle la lecture |
| `/replay speed <0.25–4>` | Vitesse de lecture |

Tous les détails sont sur [Practice](../jouer/practice.md).

## 🧰 Utilitaires

| Commande | Effet |
| --- | --- |
| `/craft` | Ouvre une table de craft |
| `/anvil` | Ouvre une enclume |
| `/ec` | Ouvre votre coffre de l'End |
| `/hat` | Porte l'objet tenu sur la tête |
| `/near` | Liste les joueurs proches |
| `/ping` | Affiche votre latence |

## 👑 Commandes liées à un grade

| Commande | Grade requis | Effet |
| --- | --- | --- |
| `/feed` | VIP | Restaure votre faim |
| `/nick` | Prestige | Pseudo aléatoire |
| `/unnick` | Prestige | Retire votre pseudo d'emprunt |
| `/fly` | Légende | Vol dans les zones autorisées |

Détail des grades sur [Rangs et grades](../le-serveur/rangs-et-grades.md).

{% hint style="info" %}
`/fly` n'est pas disponible dans les modes compétitifs : ce serait un avantage de jeu.
{% endhint %}
