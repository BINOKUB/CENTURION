# 🛡️ CENTURION - Coffre-fort Cryptographique Local

**Centurion** est une application de bureau sécurisée conçue pour stocker et protéger vos fichiers sensibles (photos, vidéos, mots de passe) de manière 100% locale et autonome. Fuyez les failles des services cloud : avec Centurion, vous êtes le seul maître de vos clés.

![Centurion Banner](assets/logo.png) ## ✨ Fonctionnalités Principales

*  **Chiffrement Militaire (AES-256) :** Tous les fichiers importés sont chiffrés et rendus illisibles pour le système d'exploitation. Sans le mot de passe maître, les données sont inexploitables.
*  **Galerie Multimédia Fluide :** Affichage moderne sous forme de tuiles. Les miniatures des images et des vidéos sont générées automatiquement lors de l'importation pour une navigation ultra-rapide sans surcharger la mémoire.
*  **Déchiffrement "In-Memory" (Zéro Trace) :** Lorsque vous consultez un fichier, celui-ci est déchiffré à la volée directement dans la mémoire vive (RAM) de l'ordinateur. **Aucun fichier temporaire n'est jamais écrit ou laissé sur le disque dur.**
*  **Importation de Masse :** Importez des dossiers entiers de médias et de documents en un seul clic.
*  **Exportation Sécurisée :** Récupérez vos fichiers originaux hors du coffre à tout moment.
*  **Verrouillage Automatique :** Le système se verrouille de lui-même et purge la mémoire vive après 5 minutes d'inactivité (clavier/souris).
*  **Moteur de Recherche Global :** Retrouvez un secret instantanément parmi toutes vos catégories.
*  **100% Portable & Hors-Ligne :** Aucune connexion Internet requise, aucune création de compte, aucun serveur cloud. L'application peut être exécutée directement depuis une clé USB.

## Architecture Technique (Aperçu)

Bien que le code source de Centurion soit **fermé et propriétaire**, son architecture repose sur des standards industriels éprouvés :
* **Moteur :** [Electron] pour des performances optimales sur environnement de bureau (Windows/Mac).
* **Cryptographie :** Algorithme `aes-256-cbc` avec génération de vecteur d'initialisation (IV) unique pour chaque fichier chiffré.
* **Traitement Multimédia :** Moteur natif pour le traitement des images lourdes et lecteur fantôme basse consommation pour l'extraction de miniatures vidéo.

##  Utilisation (Version Portable)

1. Téléchargez la dernière version de `Centurion.exe`.
2. Placez l'exécutable dans un dossier sécurisé ou sur une clé USB.
3. Lancez l'application. Au premier démarrage, cliquez sur "Créer un nouveau coffre" pour générer votre fichier `.vault` et votre dossier de données sécurisé.

##  Roadmap
* **Phase 1 :** Version Desktop Windows/Mac - *Complétée* 
* **Phase 2 :** Centurion Mobile - Développement d'une version native compagnon (iOS/Android) pour consulter ses coffres sur smartphone.

##  Avertissement de Sécurité
Centurion a été conçu selon le principe de la "Connaissance Zéro" (Zero-Knowledge). **Il n'y a aucune procédure de récupération de mot de passe ni de "porte dérobée" (backdoor).** Si vous perdez votre mot de passe maître, vos données seront irrémédiablement perdues. Conservez votre clé en lieu sûr.

---
*© 2024 Centurion - Tous droits réservés. La distribution et la modification du code source sont strictement interdites sans autorisation.*
