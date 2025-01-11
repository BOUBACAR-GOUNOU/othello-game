# Othello Game Application

## Description
Cette application est une implémentation du jeu Othello (aussi connu sous le nom de Reversi). C'est un jeu de plateau à deux joueurs se jouant sur une grille 8x8.

Le jeu d'Othello est un jeu de stratégie qui se joue sur un plateau de 64 cases. Les joueurs placent des pièces bicolores (noir d'un côté, blanc de l'autre) et doivent retourner les pièces adverses en les encadrant. Le gagnant est celui qui a le plus de pièces de sa couleur à la fin de la partie.

## Prérequis
- Java JDK 11 ou supérieur
- JavaFX


## Installation
1. Clonez le dépôt
2. Assurez-vous que toutes les dépendances sont présentes dans votre projet
3. Compilez le projet
4. Exécutez la classe `OthelloApplication`

## Structure de l'Interface
L'interface du jeu comporte plusieurs éléments :

### Barre Supérieure
- Un champ d'information général
- Affichage du joueur actuel
- Scores des deux joueurs

### Zone de Jeu
- Grille 8x8 pour le plateau de jeu

### Barre Inférieure
- Bouton "New Game" : Démarre une nouvelle partie
- Bouton "Undo" : Annule le dernier coup
- Bouton "Redo" : Rétablit le dernier coup annulé
- Bouton "AI Mode" : Active/Désactive le mode IA

## Architecture du Projet

### Structure des Dossiers

```plaintext
othello-game/
├── src/
│   └── fr/
│       └── univ_amu/
│           └── m1info/
│               └── board_game_library/
│                   ├── OthelloApplication.java
│                   ├── controller/
│                   │   └── OthelloController.java
│                   ├── model/
│                   │   ├── OthelloBoard.java
│                   │   ├── OthelloMove.java
│                   │   └── OthelloPlayer.java
│                   └── graphics/
│                       └── configuration/
│                           ├── BoardGameConfiguration.java
│                           ├── BoardGameDimensions.java
│                           ├── LabeledElementConfiguration.java
│                           ├── LabeledElementKind.java
│                           └── Position.java
├── resources/
│   └── styles/
│       └── othello-styles.css
├── test/
│   └── fr/
│       └── univ_amu/
│           └── m1info/
│               └── board_game_library/
│                   └── test/
│                       ├── OthelloBoardTest.java
│                       └── OthelloControllerTest.java
├── lib/
│   └── board_game_library.jar
├── README.md
├── LICENSE
└── pom.xml
```

### Description des Composants Principaux

#### 1. Package Principal (`fr.univ_amu.m1info.board_game_library`)

- **OthelloApplication.java** : Point d'entrée de l'application

#### 2. Package Controller

- **OthelloController.java** : Gère la logique du jeu et les interactions

#### 3. Package Model

- **OthelloBoard.java** : Représentation du plateau de jeu
- **OthelloMove.java** : Gestion des mouvements
- **OthelloPlayer.java** : Gestion des joueurs

#### 4. Package Graphics/Configuration

- **BoardGameConfiguration.java** : Configuration générale du jeu
- **BoardGameDimensions.java** : Dimensions du plateau
- **LabeledElementConfiguration.java** : Configuration des éléments d'interface
- **LabeledElementKind.java** : Types d'éléments d'interface
- **Position.java** : Gestion des positions

#### 5. Resources

- **othello-styles.css** : Styles CSS pour l'interface

#### 6. Tests

- **OthelloBoardTest.java** : Tests unitaires pour le plateau
- **OthelloControllerTest.java** : Tests unitaires pour le contrôleur

#### 7. Fichiers de Configuration

- **pom.xml** : Configuration Maven du projet
- **README.md** : Documentation du projet
- **LICENSE** : Licence du projet

## Caractéristiques de l'Architecture

- Architecture MVC (Model-View-Controller)
- Séparation claire des responsabilités
- Tests unitaires intégrés
- Configuration externalisée
- Styles CSS séparés

## Développement

Pour étendre ou modifier l'application :

1. Le fichier principal est `OthelloApplication.java`
2. La configuration de l'interface peut être modifiée dans la méthode `main`
3. La logique du jeu est gérée dans `OthelloController`

## Dépendances Externes

- `board_game_library.jar` (bibliothèque principale)
- JavaFX (interface graphique)


## Contributeurs

- **ALLOKPENOUDJI Clairemode Placida Sètchémè**
- **DIA Mouhamadou Afiss**
- **Boubacar GOUNOU**
- **OUATTARA Sie**

## Remerciements

- Ce projet a été réalisé dans le cadre d'un travail pratique visant à approfondir les compétences en Java et en Gestion du projet Informatique à l'**Université d'Aix-Marseille** (AMU).  
- Le plan de ce TP a été proposé par **F.-X. Dupé, A. Labourel, J. L. Massat**, tous enseignant à l'Université d'Aix-Marseille.  


