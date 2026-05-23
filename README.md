# Prompt Collection

Ce dépôt rassemble des prompts destinés aux LLM ainsi que des pages web simples qui servent d'aides à la génération, à la composition ou à l'adaptation de prompts.

Pour l'instant, le contenu est centré sur la génération de rétrospectives agiles. D'autres familles de prompts pourront être ajoutées par la suite sur d'autres sujets.

## Objectif du dépôt

- Centraliser des prompts réutilisables.
- Conserver des variantes et déclinaisons de prompts par thème ou par format.
- Proposer des interfaces HTML légères pour faciliter la génération de prompts.
- Publier ces aides en ligne via GitHub Pages.

## Contenu actuel

Le dépôt contient actuellement des prompts et outils autour des rétrospectives.

### Rétrospectives

- `retro/retro-meta-prompt.txt`
  Prompt de base pour générer un template de rétrospective de type Speedboat.

- `retro/Speedboat/speedboat-variation.txt`
  Variante de prompt pour adapter la structure Speedboat à un thème donné.

- `retro/Speedboat/speedboat-variation-composition.txt`
  Variante enrichie pour générer une composition thémifiée en s'appuyant sur la structure Speedboat.

- `retro/TroisPetitsCochons/troisPetitsCochonsDeLEspaces.txt`
  Exemple de prompt thématique pour une rétrospective inspirée des Trois Petits Cochons dans l'espace.

### Outils HTML

- `index.html`
  Page d'accueil du site publié via GitHub Pages.

- `retro/Speedboat/themification/index.html`
  Générateur interactif permettant de remplir les paramètres d'une variante thémifiée de Speedboat.

## Structure du dépôt

```text
.
├── index.html
├── README.md
└── retro/
    ├── retro-meta-prompt.txt
    ├── Speedboat/
    │   ├── speedboat-variation.txt
    │   ├── speedboat-variation-composition.txt
    │   └── themification/
    │       ├── index.html
    │       └── assets/
    └── TroisPetitsCochons/
        └── troisPetitsCochonsDeLEspaces.txt
```

## Utilisation

### Lire les prompts

Les fichiers texte du dépôt peuvent être ouverts tels quels, puis copiés dans l'outil LLM ou l'outil de génération d'images de votre choix.

### Utiliser les pages HTML

La page d'accueil du dépôt sert de porte d'entrée vers les aides disponibles.

Exemples actuels :

- page d'accueil : `index.html`
- générateur Speedboat thémifié : `retro/Speedboat/themification/index.html`

## GitHub Pages

Le dépôt est prévu pour être publié avec GitHub Pages.

Une fois GitHub Pages activé sur la branche principale, la page racine `index.html` devient le point d'entrée du site et permet d'accéder aux pages plus profondes du dépôt.

URL actuellement servie pour le générateur Speedboat thémifié :

https://agileanddevopstoolkit.github.io/prompt-collection/retro/Speedboat/themification/index.html

## Lancer en local

Depuis la racine du dépôt, vous pouvez servir le site avec un serveur HTTP simple :

```bash
python3 -m http.server 8080
```

Puis ouvrir dans votre navigateur :

```text
http://localhost:8080
```

## Philosophie

Le dépôt est organisé de façon simple :

- les prompts bruts restent lisibles et versionnables en texte ;
- les outils HTML restent légers, statiques et faciles à héberger ;
- chaque nouveau sujet peut être ajouté progressivement sans remettre en cause la structure existante.

## Évolutions prévues

Le dépôt a vocation à s'élargir avec le temps, par exemple :

- autres formats de rétrospectives ;
- autres générateurs de prompts ;
- autres domaines d'usage des LLM au-delà des rétrospectives ;
- pages d'aide supplémentaires accessibles depuis la page d'accueil.
