# <img src="logo.png" height="50px" weight="50px" style="margin-right: 10px; vertical-align: middle;"> CENTURION - Coffre-fort Cryptographique Local

**Centurion est une application de bureau sécurisée à hautes performances, conçue pour stocker et protéger vos fichiers sensibles (médias, documents, mots de passe) de manière 100% locale et autonome. Fuyez les failles des services cloud : avec Centurion, vous êtes le seul maître de vos clés.

##  Fonctionnalités Principales

* **Chiffrement Militaire (AES-256) :** Tous les fichiers importés sont chiffrés et rendus illisibles pour le système d'exploitation. Sans le mot de passe maître, les données sont inexploitables.
* **Performances Industrielles (Données Massives) :** Grâce à son architecture basée sur des flux continus (Streams), Centurion est capable de chiffrer, déchiffrer et sauvegarder des dizaines de Gigaoctets (Go) de données en quelques minutes, sans jamais saturer la mémoire vive (RAM) de l'ordinateur.
* **Déchiffrement "In-Memory" (Zéro Trace) :** Lorsque vous consultez un fichier lourd (ex: un film HD de 3 Go), celui-ci est déchiffré à la volée, milliseconde par milliseconde, directement dans la mémoire vive. Aucun fichier temporaire n'est jamais écrit ou laissé sur le disque dur.
* **Sauvegarde Éclair (Backup Direct) :** Créez une archive `.zip` complète de votre coffre en un clic. Le moteur de sauvegarde contourne la RAM pour des exports massifs (plus de 15 Go par minute selon votre disque SSD).
* **Importation de Masse :** Importez des dossiers entiers de médias et de documents d'un seul coup. Les miniatures sont générées automatiquement.
* **Verrouillage Automatique & Bouclier Anti-Brute-Force :** Le système se verrouille de lui-même et purge la mémoire après 5 minutes d'inactivité.
* **100% Portable & Hors-Ligne :** Aucune connexion Internet, aucun compte, aucun serveur.

## 🗂️ Formats Pris en Charge

Centurion agit comme un véritable trou noir sécurisé et peut engloutir tous les formats standards :
* **Vidéos (Lecture fluide intégrée) :** `.mp4`, `.mkv`, `.webm`, `.avi`, `.mov`, `.m4v`, etc.
* **Images (Galerie HD) :** `.jpg`, `.png`, `.webp`, `.gif`, `.svg`, `.bmp`, `.tiff`.
* **Audio :** `.mp3`, `.wav`, `.flac`, `.m4a`.
* **Documents :** `.pdf`, `.doc/docx`, `.xls/xlsx`, `.txt`, `.csv`.
* **Archives :** `.zip`, `.rar`, `.7z`.

## Architecture Technique (Aperçu)

Bien que le code source de Centurion soit **fermé et propriétaire**, son architecture repose sur des standards industriels éprouvés :
* **Moteur :** [Electron] pour des performances optimales sur environnement de bureau (Windows/Mac).
* **Cryptographie :** Algorithme `aes-256-cbc` avec génération de vecteur d'initialisation (IV) unique pour chaque fichier chiffré.
* **Traitement Multimédia :** Moteur natif pour le traitement des images lourdes et lecteur fantôme basse consommation pour l'extraction de miniatures vidéo.


## 🔐 Avertissement de Sécurité (Zero-Knowledge)

Centurion a été conçu selon le principe de la "Connaissance Zéro". **Il n'y a aucune procédure de récupération de mot de passe ni de "porte dérobée" (backdoor).** Si vous perdez votre mot de passe maître, vos données seront mathématiquement et irrémédiablement perdues. Conservez votre clé en lieu sûr. 

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
