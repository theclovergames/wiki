---
description: Référence complète des commandes joueur de Clover Games.
---

# Toutes les commandes

Toutes les commandes de cette page sont accessibles à **tous les joueurs**, sauf celles marquées d'un grade. Les commandes réservées au staff ne sont pas documentées ici.

{% hint style="info" %}
Perdu ? `/help` en jeu donne l'aide contextuelle, et `/rules` rappelle le [Règlement](reglement.md).
{% endhint %}

## Essentiel

| Commande | Effet |
| --- | --- |
| `/help` | Aide générale |
| `/rules` | Rappel du règlement |
| `/spawn` | Retour au point de départ |
| `/warp` | Accès aux destinations du serveur |
| `/rtp` | Téléportation aléatoire |
| `/back` | Retour à votre position précédente |
| `/afk` | Vous signale comme absent |
| `/discord` | Lien vers le Discord |
| `/site` | Lien vers le site |

{% hint style="warning" %}
Le temps passé en **AFK ne rapporte aucun crédit**. Voir [Crédits](credits-economie.md#gagner-des-credits).
{% endhint %}

## Téléportation entre joueurs

| Commande | Effet |
| --- | --- |
| `/tpa <joueur>` | Demande à vous téléporter chez un joueur |
| `/tpahere <joueur>` | Demande à un joueur de venir chez vous |
| `/tpaccept` | Accepte une demande reçue |
| `/tpdeny` | Refuse une demande reçue |
| `/tptoggle` | Bloque ou débloque les demandes entrantes |

## Communication

| Commande | Effet |
| --- | --- |
| `/msg <joueur> <message>` | Message privé |
| `/r <message>` | Répond au dernier message privé reçu |
| `/ignore <joueur>` | Ignore un joueur |
| `/party` | Gestion de votre groupe |

## Économie

| Commande | Effet |
| --- | --- |
| `/balance` | Votre solde de crédits — alias `/bal`, `/money` |
| `/balance <joueur>` | Solde d'un autre joueur |
| `/pay <joueur> <montant>` | Transfère des crédits |

{% hint style="danger" %}
`/pay` est immédiat et définitif. Vérifiez le pseudo et le montant.
{% endhint %}

## Progression

| Commande | Effet |
| --- | --- |
| `/leveling` | Vos niveaux, votre XP et vos récompenses |
| `/challenges` | Défis quotidiens et hebdomadaires |
| `/playtime` | Votre temps de jeu et vos paliers |
| `/vote` | Sites de vote, paliers et classement |
| `/vote rewards` | Réclame vos paliers de vote |
| `/vote top [alltime]` | Classement mensuel ou général |

## Practice

| Commande | Effet |
| --- | --- |
| `/practice` | Menu du mode Practice |
| `/practice join <ranked\|unranked> <1v1\|2v2> <kit>` | Rejoint une file |
| `/practice leave` | Quitte la file ou abandonne |
| `/practice stats [joueur] [kit] [format]` | Statistiques |
| `/practice top <kit> <format>` | Classement d'un kit |
| `/practice history` | Vos 63 derniers combats |
| `/practice effect [set <id>]` | Effets de victoire |
| `/duel <joueur> <kit>` | Défie un joueur |
| `/duel accept` · `/duel deny` | Répond à un défi |
| `/team split <kit>` | Répartit votre groupe en deux camps |
| `/botfight <kit> [easy\|normal\|hard\|expert]` | Entraînement contre un bot |
| `/replay list` | Vos replays |
| `/replay watch <id>` | Lance un replay |
| `/replay pause` · `/replay stop` | Contrôle la lecture |
| `/replay speed <0.25–4>` | Vitesse de lecture |

Tous les détails sont sur [Practice](practice.md).

## Utilitaires

| Commande | Effet |
| --- | --- |
| `/craft` | Ouvre une table de craft |
| `/anvil` | Ouvre une enclume |
| `/ec` | Ouvre votre coffre de l'End |
| `/hat` | Porte l'objet tenu sur la tête |
| `/near` | Liste les joueurs proches |
| `/ping` | Affiche votre latence |
| `/scoreboard toggle` | Affiche ou masque le tableau latéral |

## Commandes liées à un grade

| Commande | Grade requis | Effet |
| --- | --- | --- |
| `/feed` | VIP | Restaure votre faim |
| `/nick` | Prestige | Pseudo aléatoire |
| `/fly` | Légende | Vol dans les zones autorisées |

Détail des grades sur [Rangs et grades](rangs-et-grades.md).

{% hint style="info" %}
`/fly` n'est pas disponible dans les modes compétitifs : ce serait un avantage de jeu.
{% endhint %}

## Sans commande

Certaines fonctions passent par les menus en jeu plutôt que par une commande :

- **Familiers** et **gadgets** cosmétiques ;
- **Visibilité** des autres joueurs (tous, amis et groupe, personne) ;
- **Amis** et présence sur le réseau ;
- **Homes** personnels — 1 par défaut, 3 avec VIP, 5 avec Légende ;
- **Double saut** dans le lobby ;
- **Caisses** et clefs obtenues par les votes et les niveaux.

Ces menus sont accessibles depuis les items de votre barre rapide au spawn.
