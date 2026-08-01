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
| `/back` | `/retour` | Retour à votre position précédente, ou au lieu de votre mort. Créatif et Survie uniquement |
| `/afk` | | Vous signale comme absent |
| `/discord` | | Lien vers le Discord |
| `/site` | | Lien vers le site |
| `/annonces` | `/announcements`, `/ann` | Active ou coupe les annonces automatiques du chat, pour vous seul |
| `/lier` | `/link` | Affiche un code pour lier votre compte au site et à Discord |
| `/lier annuler` | | Invalide le code en cours |
| `/report <joueur> <raison>` | `/signaler` | Signale un joueur au staff |
| `/clovermenu` | | Ouvre les menus Clover |

{% hint style="warning" %}
Le temps passé en **AFK ne rapporte aucun crédit** et suspend votre progression. Voir [Crédits](../le-serveur/credits-economie.md#gagner-des-credits).
{% endhint %}

`/back` n'est disponible que sur le **Créatif**, et le sera sur la **Survie** à son ouverture. Les modes de combat en sont exclus : revenir sur le lieu de sa mort y serait un avantage de jeu.

La commande retient vos morts et vos téléportations importantes, mais cet historique **ne survit pas à un redémarrage du serveur**.

`/report` fonctionne même si le joueur visé est **hors ligne**, et il est valable sur tout le réseau. Voir [Support et signalements](../le-serveur/support-et-signalements.md#depuis-le-jeu-avec-report).

`/lier` génère un code valable 10 minutes, à saisir sur le [site](../le-serveur/le-site-web.md#lier-votre-compte-minecraft) ou sur [Discord](../le-serveur/bot-discord.md#lier-votre-compte-minecraft).

{% hint style="info" %}
Le serveur diffuse régulièrement des **annonces automatiques** dans le chat : vote, Discord, cosmétiques, boutique et aide. Si elles vous dérangent, `/annonces` les coupe **pour vous seul**, et la même bascule existe dans votre menu profil.

Elles ne vous sont de toute façon jamais envoyées pendant un match ni lorsque vous êtes AFK.
{% endhint %}

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

Le Coinflip se mise en **jetons**, jamais en crédits.

| Commande | Effet |
| --- | --- |
| `/coinflip` | Menu des annonces |
| `/coinflip claim` | Recharge quotidienne de 25 jetons |
| `/coinflip create <mise> <face\|pile>` | Publie une annonce |
| `/coinflip accept <id>` | Accepte une annonce |
| `/coinflip cancel` | Annule votre annonce |
| `/coinflip echange <jetons>` | Convertit vos jetons en crédits |
| `/coinflip list` | Annonces ouvertes |
| `/coinflip stats` | Portefeuille et statistiques |
| `/coinflip verifier <id>` | Vérifie le tirage d'un duel passé |

`/coinflip echange` convertit à raison de **100 jetons pour 1 crédit**, par multiples de 100, à partir de 500 jetons et dans la limite de 10 crédits par jour. L'inverse est impossible : un crédit ne redevient jamais un jeton.

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
| `/gadget unequip <famille\|all>` | Retire un cosmétique, ou tous |
| `/gadget favorite <id>` | Ajoute un cosmétique à vos favoris |
| `/gadget loadout <list\|save\|apply\|delete> <1-3> [nom]` | Vos trois panoplies enregistrées |
| `/doublejump` | Active ou désactive votre double saut |
| `/scoreboard` | Affiche ou masque le tableau latéral |

### Renvoyer un familier

Le menu `/pets` comporte une entrée **Renvoyer le familier**, qui range d'un clic celui qui vous suit. Elle reste visible mais grisée si aucun familier n'est invoqué.

Les 21 familiers tiennent sur une seule page, et le comparateur au centre du menu bascule le tri entre **nom** et **rareté**, pour la durée de votre session.

### Retirer un cosmétique

Dans le menu des cosmétiques, l'entrée de retrait offre deux gestes : le **clic droit** déséquipe tout d'un coup, le **clic gauche** ouvre un écran qui montre ce que vous portez, famille par famille : auras, sillages, reliques, chapeaux, jouets et accessoires de dos.

Chaque emblème y affiche le cosmétique réellement équipé : clic gauche pour l'enlever, clic droit pour parcourir le reste de la famille. Un raccourci **Panoplies** permet de tout remettre juste après.

{% hint style="info" %}
Les **signatures** n'apparaissent pas dans cet écran : elles se jouent, elles ne s'équipent pas, il n'y a donc rien à retirer.
{% endhint %}

Vos cosmétiques s'activent **dans tous les mondes du réseau**. Deux exceptions : le Practice les suspend pendant un match, pour ne pas fausser un duel.

Chaque jouet a son propre **temps de recharge**, cinq secondes en général. Pendant ce délai, l'objet affiche le balayage habituel d'une perle de l'Ender et une activation est refusée avec `Recharge : Xs` en barre d'action.

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

## 🏗️ Créatif

| Commande | Effet |
| --- | --- |
| `/plot auto` | Vous attribue la première parcelle libre |
| `/plot claim` | Réclame la parcelle où vous êtes |
| `/plot home` | Retour à votre parcelle |
| `/plot visit <joueur>` | Visite la parcelle d'un joueur |
| `/plot info` | Informations sur la parcelle |
| `/plot trust <joueur>` | Accès complet, même en votre absence |
| `/plot add <joueur>` | Accès pendant que vous êtes connecté |
| `/plot remove <joueur>` | Retire un accès |
| `/plot deny <joueur>` | Interdit l'accès à un joueur |
| `/plot setbiome <biome>` | Change le biome de votre parcelle |
| `/plot delete` | Supprime votre parcelle, définitivement |
| `/plot help` | Liste complète en jeu |

{% hint style="warning" %}
Écrivez `/plot` en entier : `/p` est le raccourci de `/party`, y compris sur le Créatif.
{% endhint %}

Tous les détails sont sur [Créatif](../jouer/creatif.md).

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
