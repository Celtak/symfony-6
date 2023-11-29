# Étapes

## 1. Créer un projet

```bash
git clone https://github.com/Celtak/symfony-6
```

## 2. Aller dans le dossier du projet

```bash
cd symfony-6
```

## 3. Installer les dépendances

```bash
composer install
```

## 4. Ne pas inclure la configuration de Docker proposé par Symfony

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

## 5. Modifier le fichier `.env` pour la connexion à la base de données

```yml
DATABASE_URL=postgresql://user:userpass@127.0.0.1:5432/symfonydb?serverVersion=15&charset=utf8
```

## 6. Lancer le serveur local

```bash
symfony server:start
```
