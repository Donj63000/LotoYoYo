# LotoYoYo

LotoYoYo est une application Java permettant de générer et d'analyser des grilles de pronostics sportifs. Elle fournit un ensemble d'outils pour estimer la couverture de vos tickets, calculer leurs probabilités de réussite et générer automatiquement des combinaisons optimisées.

## Fonctionnalités principales

- **Création de grilles personnalisées** : choisissez pour chaque match les issues possibles (`1`, `N`, `2`).
- **Gestion des cotes** : saisissez les cotes de chaque résultat et laissez le logiciel calculer les probabilités associées.
- **Calculs statistiques** : nombre total de tickets, coût, couverture des scénarios, distribution des bons pronostics, worst‑case, espérance, écart‑type, etc.
- **Auto‑Grille** : génération automatique d'un ensemble de tickets pertinents à partir des cotes et des issues sélectionnées.
- **Interface sombre moderne** : basée sur Swing, FlatLaf et MigLayout.
- **Bouton de thème** : permet de basculer entre le thème sombre et un thème bleu/blanc.
- **Aide intégrée** : une fenêtre d'aide détaillée explique le fonctionnement du logiciel.

## Prérequis

- Java 17 ou supérieur (SDK d'Oracle).
- Maven (facultatif si vous utilisez directement le JAR fourni).

## Installation de Java

Si Java n'est pas encore installé sur votre machine, voici la procédure la
plus simple selon votre système :

### Windows

1. Rendez-vous sur le [site d'Oracle](https://www.oracle.com/java/technologies/downloads/) et
   téléchargez l'installeur du **JDK 17** pour Windows.
2. Exécutez le fichier obtenu puis suivez les options par défaut.
3. Ouvrez une nouvelle invite de commandes et vérifiez l'installation avec
   `java -version`.

### macOS

1. Téléchargez le paquet **JDK 17** pour macOS depuis le [site d'Oracle](https://www.oracle.com/java/technologies/downloads/).
2. Ouvrez l'image disque et lancez l'installateur.
3. Une fois l'installation terminée, ouvrez un nouveau terminal et vérifiez avec
   `java -version`.

### Linux (Ubuntu/Debian)

1. Téléchargez l'archive **JDK 17** adaptée à votre système sur le [site d'Oracle](https://www.oracle.com/java/technologies/downloads/).
2. Décompressez-la dans le répertoire de votre choix (par exemple `/opt/java`).
3. Ajoutez le chemin `bin` de cette installation à votre `PATH` puis vérifiez
   la version avec `java -version`.

Ces étapes vous permettent d'obtenir Java 17 (ou une version plus récente),
nécessaire pour lancer LotoYoYo.

## Compilation

Pour construire le projet à partir des sources :

```bash
mvn package
```

Le JAR final `LotoYoYo.jar` sera généré dans le répertoire `target/`.

## Développement avec IntelliJ IDEA

Pour modifier le code source ou contribuer au projet, vous pouvez utiliser **IntelliJ IDEA** :

1. Installez [IntelliJ IDEA](https://www.jetbrains.com/idea/download/) dans sa version Community ou Ultimate.
2. Dans la fenêtre d'accueil, choisissez **Open** et sélectionnez le dossier contenant ce dépôt (ou directement le fichier `pom.xml`).
3. L'IDE importe alors le projet Maven et télécharge automatiquement les dépendances nécessaires.
4. Le code se trouve sous `src/main/java`. Modifiez les fichiers souhaités puis utilisez le menu **Build > Build Project** pour compiler.
5. Vous pouvez créer une configuration d'exécution afin de lancer l'application depuis IntelliJ.

## Exécution

Lorsque Java est installé, téléchargez le fichier `LotoYoYo.jar` (inclus dans ce
dépôt) puis suivez ces étapes :

1. Ouvrez un terminal (ou l'invite de commandes sous Windows).
2. Placez-vous dans le répertoire contenant `LotoYoYo.jar` :
   ```bash
   cd /chemin/vers/le/dossier
   ```
3. Lancez l'application :
   ```bash
   java -jar LotoYoYo.jar
   ```

L'application se lance alors en plein écran et vous permet d'ajouter des
grilles via le bouton **Ajouter**.

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

LotoYoYo a été développé par DonJ avec l'aide d'une IA (JetBrains). Vos retours et contributions sont les bienvenus !
