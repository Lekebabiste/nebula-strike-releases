# Nebula Strike

Combat spatial en vue de dessus, en pixel art, avec une physique de glisse « patinoire ». Jusqu'à 4 pilotes,
en local contre des bots ou en ligne avec des amis.

**Ce dépôt ne contient que les exécutables.** Téléchargez la dernière version dans
[Releases](../../releases/latest) :

| Système | Fichier | Lancer |
|---|---|---|
| Windows 10 / 11 | `NebulaStrike-vX.Y.Z-windows-x64.zip` | décompresser, puis `nebula_strike.exe` |
| Linux (x86-64, glibc ≥ 2.34) | `NebulaStrike-vX.Y.Z-linux-x64.tar.gz` | `tar -xzf` puis `./nebula_strike` (bibliothèque `sdl2` requise) |

Chaque archive contient le jeu, le **serveur dédié** (`nebula_server`) et le dossier `assets/`.

## Modes de jeu

Survie (vagues, boss), Combat (chacun pour soi ou en équipes), Capture du drapeau, Course sur circuit,
Capture de territoire. Bots, armes aléatoires, 10 armes spéciales, dash, drone, trous de ver.
Vaisseau personnalisable (pseudo, couleur, forme) ; jeu en français, anglais, japonais, russe et arabe.

## Jouer en ligne

Un joueur choisit « Héberger une partie en ligne » (port UDP 27015), les autres « Rejoindre » avec son
adresse ; les serveurs déjà rejoints sont mémorisés. Pour un serveur permanent :
`./nebula_server --mode course --bots 2` (voir `--help`).

## Mises à jour

Le jeu vérifie au lancement s'il existe une version plus récente et propose de l'installer
(Entrée : télécharger et redémarrer, Échap : plus tard). `NEBULA_NO_UPDATE=1` désactive la vérification.
