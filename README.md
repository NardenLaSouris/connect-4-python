# Connect-4-Python

Puissance 4 pour deux joueurs avec interface graphique Tkinter, écrit en Python au lycée pour pratiquer la programmation orientée objet.

## Fonctionnement

- Grille de 7 colonnes sur 6 lignes dessinée dans une fenêtre Tkinter.
- On choisit la colonne avec les boutons 1 à 7, puis on clique sur **Jouer** : le pion tombe à la première case libre.
- La couleur qui commence (rouge ou jaune) est tirée au hasard, et l'interface indique à qui c'est le tour.
- Après chaque coup, le programme cherche un alignement de 4 pions à l'horizontale, à la verticale ou en diagonale. En cas de victoire, le bouton **Jouer** se désactive.

## Lancer le jeu

Python 3 avec Tkinter (inclus dans l'installation standard sous Windows et macOS ; sous Linux : `sudo apt install python3-tk`).

```bash
git clone https://github.com/NardenLaSouris/connect-4-python.git
cd connect-4-python
python3 "puissance 4 v2.py"
```

## Structure du code

- `Pion` : position et couleur d'un pion, et son dessin sur le canevas.
- `Grille` : plateau de 7 × 6, ajout d'un pion dans une colonne, détection de la victoire dans les quatre directions.
- Le reste du fichier construit la fenêtre (canevas, choix de colonne, boutons Jouer et Quitter).
