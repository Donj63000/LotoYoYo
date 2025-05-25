# LotoYoYo

LotoYoYo est une application Java permettant de générer et d'analyser des grilles de pronostics sportifs. Elle fournit un ensemble d'outils pour estimer la couverture de vos tickets, calculer leurs probabilités de réussite et générer automatiquement des combinaisons optimisées.

## Fonctionnalités principales

- **Création de grilles personnalisées** : choisissez pour chaque match les issues possibles (`1`, `N`, `2`).
- **Gestion des cotes** : saisissez les cotes de chaque résultat et laissez le logiciel calculer les probabilités associées.
- **Calculs statistiques** : nombre total de tickets, coût, couverture des scénarios, distribution des bons pronostics, worst‑case, espérance, écart‑type, etc.
- **Auto‑Grille** : génération automatique d'un ensemble de tickets pertinents à partir des cotes et des issues sélectionnées.
- **Interface sombre moderne** : basée sur Swing, FlatLaf et MigLayout.
- **Aide intégrée** : une fenêtre d'aide détaillée explique le fonctionnement du logiciel.

## Prérequis

- Java 17 ou supérieur.
- Maven (facultatif si vous utilisez directement le JAR fourni).

## Compilation

Pour construire le projet à partir des sources :

```bash
mvn package
```

Le JAR final `LotoYoYo.jar` sera généré dans le répertoire `target/`.

## Exécution

Si vous disposez déjà du JAR (présent dans ce dépôt), lancez simplement :

```bash
java -jar LotoYoYo.jar
```

L'application se lance en plein écran et vous permet d'ajouter des grilles via le bouton **Ajouter**.

## Utilisation rapide

1. Indiquez le nombre de matchs souhaité dans le champ "Matches" puis cliquez sur **Ajouter** pour créer une nouvelle grille.
2. Sélectionnez pour chaque match les résultats que vous souhaitez couvrir (1 / N / 2).
3. Renseignez les cotes dans la section *Cotes* puis cliquez sur **Appliquer cotes** pour mettre à jour les probabilités.
4. Cliquez sur **Calculer** pour afficher l'ensemble des statistiques liées à la grille courante.
5. Utilisez la fonction **Auto‑Grille** pour générer automatiquement des tickets optimisés selon vos sélections et probabilités.
6. Le bouton **Aide** de la fenêtre principale ouvre un guide complet expliquant toutes les options disponibles.

## Licence

Ce projet est distribué sous licence MIT. Voir le fichier [`src/main/java/org/example/license`](src/main/java/org/example/license) pour le texte complet.

## Remerciements

LotoYoYo a été développé par Valentin Gidon avec l'aide d'une IA (JetBrains). Vos retours et contributions sont les bienvenus !
