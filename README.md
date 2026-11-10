# Python Image Tools

Quatre petits scripts Python pour jouer avec les pixels : transformer des images avec Pillow, et un morpion à jouer contre une IA dans le terminal.

## Les scripts

| Dossier | Ce que fait le script |
|---|---|
| `Contour/` | Repère la couleur dominante de l'image (le fond) et trace en rouge les pixels qui la bordent : un contour de l'image |
| `Convertisseur_bw/` | Convertit une image en niveaux de gris en faisant la moyenne des canaux rouge, vert et bleu de chaque pixel |
| `Convertisseur_couleur/` | Recolorise une image en niveaux de gris avec une palette chaude choisie selon la luminosité, avec une part d'aléatoire |
| `Tic-Tac-Toe/` | Morpion contre l'ordinateur dans le terminal |

### Le morpion

L'IA suit une stratégie simple, dans cet ordre : gagner si elle le peut, bloquer le coup gagnant du joueur, prendre le centre, prendre un coin, puis jouer une case libre. Vous jouez les `X`, en choisissant une case de 1 à 9.

## Utilisation

Prérequis : Python 3 et Pillow.

```bash
git clone https://github.com/imene-be/python-image-tools.git
cd python-image-tools
pip install pillow

python3 Tic-Tac-Toe/ttt.py
```

Pour les trois scripts d'image, le nom du fichier à traiter et celui du fichier de sortie sont écrits à la dernière ligne du script : remplacez-les par vos propres images, puis lancez-le.

```bash
python3 Convertisseur_bw/tobw.py
```

## Ce que j'y ai travaillé

- Lecture et écriture de pixels avec Pillow
- Parcours de voisinage (détection de contour)
- Petite logique de jeu et stratégie d'IA à règles

---

Réalisé par [Imène Bentifraouine](https://imenebe.fr).
