# Namer App

Une application Flutter de génération de noms aléatoires, permettant à l'utilisateur de parcourir des paires de mots, de les ajouter à ses favoris et de consulter la liste de ses favoris.

## Fonctionnalités

- Génération de paires de mots aléatoires grâce au package [`english_words`](https://pub.dev/packages/english_words)
- Ajout et suppression de favoris
- Affichage de la liste des favoris
- Interface responsive utilisant Material 3 et `NavigationRail`
- Gestion d'état avec [`provider`](https://pub.dev/packages/provider)

## Aperçu

- **Accueil** : Affiche une paire de mots aléatoire et permet de l'ajouter ou de la retirer des favoris.
- **Favoris** : Liste toutes les paires de mots ajoutées en favoris.

## Structure principale

- [`MyApp`](lib/main.dart) : Point d'entrée de l'application, configuration du thème et du provider.
- [`MyAppState`](lib/main.dart) : Gestionnaire d'état (ChangeNotifier) pour la paire courante et la liste des favoris.
- [`MyHomePage`](lib/main.dart) : Widget principal avec navigation entre la génération et les favoris.
- [`GeneratorPage`](lib/main.dart) : Génère et affiche une nouvelle paire de mots.
- [`FavoritePage`](lib/main.dart) : Affiche la liste des favoris.
- [`BigCard`](lib/main.dart) : Widget d'affichage stylisé pour une paire de mots.

## Dépendances

- [english_words](https://pub.dev/packages/english_words)
- [provider](https://pub.dev/packages/provider)
- [flutter/material.dart](https://api.flutter.dev/flutter/material/material-library.html)

## Lancer le projet

```sh
flutter pub get
flutter run