# Pathfinding - Lee Algorithm

Programme de recherche de chemin utilisant l'algorithme de Lee.

---

## Installation

Aucune dépendance externe requise.

---

## Lancer le programme

```bash
# Avec TypeScript
ts-node main.ts simple.map

# Avec Node.js (après compilation)
node main.ts simple.map
```

---

## Format de la carte

Créez un fichier texte avec les symboles suivants :

- `S` = Point de départ (Start)
- `E` = Point d'arrivée (End)
- `.` = Chemin libre
- `o` = Obstacle (mur)

### Exemple : map.txt

```
S.....
o.ooo.
o.o...
o.oooo
.....E
```

---

## Fonctionnement

### Algorithme de Lee

1. Parcourt la carte depuis le point de départ
2. Numérote chaque case accessible
3. S'arrête quand il trouve la sortie
4. Retrace le chemin le plus court

### Résultat

Le programme affiche les coordonnées du chemin optimal :

```
0:0 0:1 0:2 1:2 2:2 2:3 2:4 3:4 4:4 4:5
```

Format : `x:y x:y x:y ...`

---

## Messages d'erreur

- `no map` - Aucun fichier fourni
- `error S not found` - Point de départ manquant
- `error E not found` - Point d'arrivée manquant
- `no way` - Aucun chemin possible

---

## Exemple d'utilisation

### Trouver le chemin

```bash
ts-node main.ts simple.map
```

### Résultat

```
0:0 0:1 0:2 1:2 2:2 2:3 2:4 3:4 4:4 4:5
```

---

## Symboles

- `S` - Start (départ)
- `E` - End (arrivée)
- `.` - Chemin libre
- `o` - Obstacle (mur)

---

Bon pathfinding !
