# Jeux Bash

Deux jeux en ligne de commande : Le Juste Prix et Le Compte est Bon.

---

## Le Juste Prix

Devinez le nombre mystère entre 1 et 50 en 15 tentatives maximum.

### Installation

```bash
nano juste_prix.sh
# Coller le code du jeu
# Sauvegarder : Ctrl + O, Entrée, Ctrl + X
chmod +x juste_prix.sh
```

### Lancer le jeu

```bash
./juste_prix.sh
```

### Règles

- Nombre entre 1 et 50
- 15 tentatives maximum
- Indication "Trop haut" ou "Trop bas"
- Validation des entrées

---

## Le Compte est Bon

Trouvez le nombre cible en utilisant les 5 nombres donnés avec les opérations.

### Installation

```bash
nano compte_bon.sh
# Coller le code du jeu
# Sauvegarder : Ctrl + O, Entrée, Ctrl + X
chmod +x compte_bon.sh
```

### Lancer le jeu

```bash
./compte_bon.sh
```

### Règles

- 5 nombres aléatoires entre 1 et 20
- Nombre cible entre 1 et 100
- 5 tentatives maximum
- Utilisez les opérations : + - * /

---

## Commandes utiles

```bash
# Créer un fichier
nano nom_fichier.sh

# Rendre exécutable
chmod +x nom_fichier.sh

# Exécuter
./nom_fichier.sh

# Voir le contenu
cat nom_fichier.sh
```

---

## Dépannage

### Permission denied

```bash
chmod +x nom_fichier.sh
```

### Fichier ne s'exécute pas

```bash
bash nom_fichier.sh
```

---

Bon jeu !
