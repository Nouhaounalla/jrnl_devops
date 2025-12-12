Le pipeline est composé de 4 jobs principaux :



1\. Test (Tests et Vérifications)

Checkout du code

Installation de Python 3.11

Installation de Poetry

Installation des dépendances

Exécution des tests avec pytest

Génération du rapport de tests HTML

2\. Build (Construction de l'image Docker)

Construction de l'image Docker

Test de l'image (vérification de la version)

Sauvegarde de l'image comme artifact

Upload vers GitHub Actions

3\. Push to Docker Hub (Optionnel)

Connexion à Docker Hub

Push de l'image vers le registre

Tag avec SHA du commit

4\. Deploy (Résumé du déploiement)

Affichage du statut final

Confirmation de la réussite

Déclencheurs du Pipeline

Le pipeline se déclenche sur :

Push sur les branches `develop` et `main`

Pull requests vers `develop` et `main`



