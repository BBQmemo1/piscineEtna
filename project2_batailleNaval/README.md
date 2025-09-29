# Bataille Navale

Jeu de bataille navale en ligne de commande pour 2 joueurs.

---

## Installation

```bash
npm install readline-sync
```

---

## Lancer le jeu

```bash
# Avec Node.js
node battleship.js 3

# Avec TypeScript
ts-node battleship.ts 3

# Le nombre 3 = nombre de bateaux par joueur
```

---

## Règles

### Placement des bateaux

- Chaque joueur place ses bateaux
- Format : `1A`, `2B`, `3C`, etc.
- Les bateaux sont cachés de l'adversaire

### Tour de jeu

- Les joueurs tirent à tour de rôle
- Format : `1A`, `2B`, `3C`, etc.
- `X` = Touché
- `M` = Manqué
- Le premier qui coule tous les bateaux gagne

---

## Grille

```
  A B C D E F G H
1 . . . . . . . .
2 . . . . . . . .
3 . . . . . . . .
4 . . . . . . . .
5 . . . . . . . .
6 . . . . . . . .
7 . . . . . . . .
8 . . . . . . . .
```

---

## Exemples

### Démarrer avec 3 bateaux

```bash
ts-node battleship.ts 3
```

### Démarrer avec 5 bateaux

```bash
ts-node battleship.ts 5
```

---

## Symboles

- `.` = Eau
- `0` = Bateau (caché)
- `X` = Touché
- `M` = Manqué

---

Bon jeu !
