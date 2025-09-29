# API Pokémon

API REST pour gérer des données Pokémon avec Express et MySQL.

---

## Installation

```bash
npm install express dotenv
npm install --save-dev @types/express @types/node typescript
```

---

## Configuration

Créer un fichier `.env` :

```env
PORT=8080
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=pokemon_db
```

Ajouter dans `package.json` :

```json
{
  "scripts": {
    "dev": "ts-node src/index.ts",
    "build": "tsc",
    "start": "node dist/index.js"
  }
}
```

---

## Lancer le serveur

```bash
# Développement
npm run dev

# Production
npm start
```

---

## Endpoints

### GET /

Retourne un message de bienvenue.

```bash
curl http://localhost:8080/
```

**Réponse :** `"hello"`

---

### GET /pokemon

Récupère tous les Pokémon.

```bash
curl http://localhost:8080/pokemon
```

**Réponse :**
```json
[
  {
    "id": 1,
    "name": "Bulbasaur",
    "type": "Grass"
  },
  ...
]
```

---

### GET /pokemon/:id

Récupère un Pokémon par son ID.

```bash
curl http://localhost:8080/pokemon/1
```

**Réponse :**
```json
{
  "id": 1,
  "name": "Bulbasaur",
  "type": "Grass"
}
```

---

### GET /type

Récupère tous les types de Pokémon.

```bash
curl http://localhost:8080/type
```

**Réponse :**
```json
[
  "Fire",
  "Water",
  "Grass",
  ...
]
```

---

### GET /type/:type

Récupère tous les Pokémon d'un type spécifique.

```bash
curl http://localhost:8080/type/Fire
```

**Réponse :**
```json
[
  {
    "id": 4,
    "name": "Charmander",
    "type": "Fire"
  },
  ...
]
```

---

## Structure

```
project/
├── src/
│   ├── index.ts
│   ├── route.ts
│   └── logger.ts
├── .env
├── package.json
└── tsconfig.json
```

---

## Modules

- **index.ts** - Point d'entrée, routes Express
- **route.ts** - Fonctions de base de données
- **logger.ts** - Système de logs

---

## Codes d'erreur

- **200** - Succès
- **500** - Erreur serveur

---

## Tester l'API

### Avec curl

```bash
# Tous les Pokémon
curl http://localhost:8080/pokemon

# Un Pokémon spécifique
curl http://localhost:8080/pokemon/25

# Tous les types
curl http://localhost:8080/type

# Pokémon par type
curl http://localhost:8080/type/Electric
```

### Avec un navigateur

```
http://localhost:8080/pokemon
http://localhost:8080/pokemon/1
http://localhost:8080/type
http://localhost:8080/type/Fire
```

---
