# Étapes

## 1. Créer un projet

```bash
git clone https://github.com/Celtak/symfony-6
```

## 2. Installer les dépendances

```bash
composer install
```

## 3. Ne pas inclure la configuration de Docker proposé par Symfony

```bash
Do you want to include Docker configuration from recipes?
    [y] Yes
    [n] No
    [p] Yes permanently, never ask again for this project
    [x] No permanently, never ask again for this project
    (defaults to y):
```

```bash
Choisir `n` ou `x`.
```

### Pourquoi ?

Nous avons déjà notre propre configuration de Docker.

## 4. Modifier le fichier `.env` pour la connexion à la base de données

```yml
DATABASE_URL=postgresql://user:userpass@postgres:5432/symfonydb?serverVersion=15&charset=utf8
```
