# SH13_karlitou
## Sherlock Holmes 13 - Jeu multijoueur en réseau
Ce projet est une implémentation du jeu "Sherlock Holmes 13" en mode multijoueur, permettant à 4 joueurs de s'affronter dans un jeu de déduction pour trouver le personnage coupable.
Compilation rapide
Pour compiler le projet, utilisez simplement:
```
	make all
```
## Exécution rapide

Lancer le serveur (dans un terminal):
bash
```
	make run_server
```

Lancer les clients (chacun dans un terminal séparé):

``` bash
	make run_client1 
	make run_client2
	make run_client3
	make run_client4
```
Démarrer la partie: Dans chaque client, cliquez sur le bouton "Connect". La partie commence automatiquement une fois que les 4 joueurs sont connectés.

## Comment jouer
```
Chaque joueur reçoit 3 cartes. Une 13ème carte est secrètement désignée comme "coupable".
À votre tour, vous pouvez:

Observer un symbole chez tous les joueurs
Demander à un joueur spécifique combien d'un certain symbole il possède
Accuser un personnage d'être le coupable
```
Le premier à identifier correctement le coupable gagne la partie!
## Prérequis techniques
```
GCC
SDL2 (avec SDL2_image et SDL2_ttf)
pthread
```
Sur Ubuntu/Debian:
```
bash
sudo apt-get install gcc make libsdl2-dev libsdl2-image-dev libsdl2-ttf-dev
```
## Structure du code
```
server.c : Serveur de jeu (logique, communication)
sh13.c : Client avec interface graphique
Makefile : Facilite la compilation et l'exécution
```
