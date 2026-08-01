# Plan de migration du wiki Clover Games

Document de travail interne : **ne pas publier sur le wiki**.

## 1. Ce qui change

| | Avant | Après |
| --- | ---: | ---: |
| Pages publiées | 60 | **12** |
| Pages vides | 36 | **0** |
| Profondeur maximale | 5 niveaux | **2 niveaux** |
| Pages titrées « Règles » | 8 | 1 |
| Pages titrées « Commandes » | 6 | 1 |
| Barèmes de sanctions concurrents | 2 | 1 |

Principe directeur : **aucune page publiée sans contenu réel**. Les pages reviennent au fil du développement.

## 2. Nouvelle arborescence

```
Découvrir
├── Bienvenue sur Clover Games      → bienvenue.md
└── Se connecter au serveur         → se-connecter.md

Le serveur
├── Règlement                       → reglement.md
├── Support et signalements         → support-et-signalements.md
├── Rangs et grades                 → rangs-et-grades.md
├── Crédits : l'économie du réseau  → credits-economie.md
└── Votes et récompenses            → votes-et-recompenses.md

Jouer
├── Les modes de jeu                → modes-de-jeu.md
├── Practice : duels et classement  → practice.md
├── PvPSoup : combat libre          → pvpsoup.md
├── Créatif                         → creatif.md
└── SkyPvP : combat libre           → skypvp.md

Référence
└── Toutes les commandes            → commandes.md
```

## 3. Sort de chaque page existante

### Remplacées (contenu repris et corrigé)

| Page actuelle | Devient |
| --- | --- |
| `/` (Bienvenue) | `bienvenue.md` + `se-connecter.md` |
| `/wiki/regles` | `reglement.md` |
| `/wiki/economies` | `credits-economie.md` |
| `/wiki/rangs` (vide) | `rangs-et-grades.md` |
| `/wiki/votes` (vide) | `votes-et-recompenses.md` |
| `/wiki/jeux-et-commandes` | `modes-de-jeu.md` |
| `/wiki/jeux-et-commandes/modes-de-jeu` | `modes-de-jeu.md` |
| `/wiki/jeux-et-commandes/modes-de-jeu/practice` (vide) | `practice.md` |
| `/wiki/jeux-et-commandes/modes-de-jeu/survie/commandes` | `commandes.md` |

### À supprimer

| Page | Raison |
| --- | --- |
| `/wiki/table-des-matieres` | Duplique la navigation générée par GitBook, et était incomplète |
| `…/survie/regles`, `…/practice/regles`, `…/pvpsoup/regles` | Vides, remplacées par le règlement unique |
| `…/skypvp/regles`, `…/bedwars/regles`, `…/skywars/regles`, `…/murder/regles` | Copies quasi identiques créant un second barème de sanctions |
| `…/evenements/donjons` | Doublon de `…/survie/donjons` : la navigation pointait sur le mauvais |
| Les 5 autres pages `Commandes` | Fusionnées dans `commandes.md` |

### À passer en brouillon (non publiées)

Elles reviendront quand le mode existera. Garder le contenu, retirer de la publication.

- **Survie** et ses 11 sous-pages (mondes, donjons, caisses, enchères, coffre de vente, marché noir, quêtes, niveaux…)
- **BedWars** et ses sous-pages : le contenu de la page principale est réutilisable
- **SkyWars** et ses sous-pages : idem
- **SkyPvP** et ses sous-pages : idem
- **PvPSoup**, **Murder**, **TheLab**
- **Practice** : sous-pages bots, divisions, classements, leur contenu est désormais dans `practice.md`
- **Événements** : donjons, pvpswap, mineral-contest, chasse-au-coffre, uhc, koth

### Redirections

**Déjà écrites** dans `.gitbook.yaml`, à la racine de ce dossier : les **62 anciennes URL** y sont redirigées vers leur équivalent, pour ne casser aucun lien existant (Discord, site, Google).

Extrait :

```yaml
redirects:
  wiki/table-des-matieres: bienvenue.md
  wiki/regles: reglement.md
  wiki/economies: credits-economie.md
  wiki/rangs: rangs-et-grades.md
  wiki/votes: votes-et-recompenses.md
  wiki/jeux-et-commandes: modes-de-jeu.md
  wiki/jeux-et-commandes/modes-de-jeu: modes-de-jeu.md
  wiki/jeux-et-commandes/evenements: modes-de-jeu.md
  wiki/jeux-et-commandes/modes-de-jeu/practice: practice.md
  wiki/jeux-et-commandes/modes-de-jeu/survie: modes-de-jeu.md
  wiki/jeux-et-commandes/modes-de-jeu/skypvp: modes-de-jeu.md
  wiki/jeux-et-commandes/modes-de-jeu/pvpsoup: modes-de-jeu.md
  wiki/jeux-et-commandes/modes-de-jeu/bedwars: modes-de-jeu.md
  wiki/jeux-et-commandes/modes-de-jeu/skywars: modes-de-jeu.md
  wiki/jeux-et-commandes/modes-de-jeu/murder: modes-de-jeu.md
  wiki/jeux-et-commandes/modes-de-jeu/thelab: modes-de-jeu.md
  wiki/jeux-et-commandes/modes-de-jeu/survie/commandes: commandes.md
```

## 4. Corrections factuelles appliquées

| Sujet | Wiki avant | Corrigé en | Source |
| --- | --- | --- | --- |
| Monnaie | Deux monnaies : « Pièces » et « Clovers » | **Une seule : Crédits** | `modules/economy.md` |
| Prix des grades | Absent | 499 / 1 299 / 1 999 / 3 499 crédits | `modules/economy.md` |
| Gratuité | « entièrement gratuit », « toutes les fonctionnalités accessibles gratuitement » | Formulation retirée ; boutique et grades payants documentés | `3. L'économie.md` |
| Conversion en euros | Absent | Mention explicite : pas de conversion ni de remboursement en argent réel | `modules/economy.md` |
| Bedrock | Crossplay annoncé, port 19132 | **Annoncé comme prévu, non certifié** | `1. Informations.md` |
| Discord | `dsc.gg/clovergames` | `discord.gg/theclovergames` | `6. Communications.md` |
| Boutique / site | Jamais liés | Liés partout où c'est utile | `1. Informations.md` |
| Sanctions | Deux barèmes concurrents | Un barème unique à 5 niveaux, valable réseau | consolidation |
| Procédure de support | « contacter le support », sans indication | Page dédiée : signalement, bug, achat, contestation | manquait |
| Commandes Survie | 8 commandes, descriptions vides ; `/claim`, `/unclaim`, `/quetes`, `/bienvenue` inexistantes | Référence unique, uniquement des commandes réellement déclarées | `permissions-par-grades.md` |
| `/quetes`, `/niveaux` | Annoncées | Vraies commandes : `/challenges`, `/leveling` | idem |
| Sites de vote | Absents | Liste-Serveurs.fr, Serveur Minecraft Vote | `modules/vote.md` |
| Orthographe | « Événements » / « Évènements » mélangés ; « SkyPvP » / « SkyPVP » | Uniformisé : **Événements**, **SkyPvP** | — |
| Placeholders | « Le monde de l'End est… », « Le donjon est… » publiés | Supprimés | — |

## 5. Décisions qui te reviennent

1. ~~**Statut du réseau.**~~ **Résolu.** Modes ouverts confirmés : **Lobby, Practice, PvPSoup, SkyPvP, Créatif**. Survie, BedWars, SkyWars, Murder et TheLab prévus, sans date. Plus aucun mode en « développement ».

   ⚠️ **`2. Fonctionnalités.md` est désormais faux** : il classe Practice en « activation requise », PvPSoup, SkyPvP et Créatif en « Envisagé ». À mettre à jour, c'est la source que je consulte.

   ✅ **Le Créatif a désormais sa page** (`jouer/creatif.md`), rédigée depuis la configuration PlotSquared de `Sauvegardes/V1.9/`, valeurs confirmées en jeu le 28 juillet 2026. Complète : 5 parcelles par joueur, confirmé le 28 juillet 2026.

   ~~**Le Créatif est ouvert mais n'a aucune page.**~~ Je n'ai trouvé aucune source exploitable : pas de config PlotSquared hors `Sauvegardes/V1.9/`, aucun module `creatif` documenté, seulement un profil d'hologrammes. Il me faut : taille et nombre de parcelles par joueur, commandes de claim et de gestion, droits d'invités, limites (redstone, entités, WorldEdit), et règles de modération des constructions.

2. **Publication de `rangs-et-grades.md`.** Ta doc interne est explicite : *« Un audit offre par offre est obligatoire avant toute vente »* et *« les avantages commerciaux annoncés dépassent parfois les permissions réellement livrées »*. La page ne documente que les avantages confirmés côté plugin (identité, homes, `/feed`, `/nick`, `/fly`, allocation mensuelle). **Ne la publie qu'après l'audit**, et vérifie qu'elle ne contredit pas les fiches de la boutique, notamment `/vip`, `/abonnement`, `/privé`, les remises cosmétiques et les limites d'amis, qui n'ont aujourd'hui aucun mécanisme technique documenté.

3. **Bedrock.** J'ai retiré l'annonce du crossplay. Si les tests sont concluants, il suffit de remplacer l'encadré de `se-connecter.md` par l'adresse et le port réels.

4. **Contradiction interne à trancher.** `2. Fonctionnalités.md` classe SkyPvP et PvPSoup en « Envisagé », alors que `modules/skypvp.md` et `modules/pvpsoup.md` existent et sont fournis. J'ai retenu « en développement ». À aligner dans ta doc interne.

5. **Deux pages restent à créer** et je ne peux pas les rédiger sans toi :
   - **FAQ** : ta doc de communication la liste comme prérequis au lancement.
   - **Journal des mises à jour** : `Changelogs/📰 Mise à Jour.txt` existe déjà et le rythme éditorial prévoit un changelog par version.

## 6. Points à vérifier en jeu

Ces commandes ne sont pas nommées explicitement dans la doc technique. Elles sont volontairement absentes des tableaux de `commandes.md` et regroupées dans la section « Sans commande ». À confirmer puis à ajouter si elles existent :

- gestion des *homes* (`/home`, `/sethome`, `/delhome` ?)
- amis (`/friends` ?)
- visibilité (`/visibility` ?)
- familiers et gadgets
- caisses

## 7. Ordre d'exécution suggéré

1. Créer les 10 nouvelles pages.
2. Passer en brouillon les pages de modes non disponibles.
3. Supprimer les doublons et la table des matières manuelle.
4. Vérifier les redirections de `.gitbook.yaml` (déjà rédigées).
5. Publier : sauf `rangs-et-grades.md`, en attente de l'audit.
6. Mettre à jour le lien du wiki dans la navbar du site et sur le Discord.
