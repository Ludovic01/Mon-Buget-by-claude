# Mon Budget — projet Android

Application de budget personnel, 100 % hors ligne (aucune permission, aucune donnée envoyée).
Les données restent sur le téléphone ; l'export CSV et la sauvegarde JSON sont enregistrés dans **Téléchargements**.

## Obtenir l'APK sans rien installer (GitHub)

1. Créez un compte gratuit sur github.com, puis un nouveau dépôt (privé ou public).
2. Envoyez-y **tout le contenu de ce dossier**, y compris le dossier caché `.github`
   (sur le site : *Add file → Upload files*, en glissant tout le dossier).
3. Ouvrez l'onglet **Actions**. La compilation démarre toute seule (environ 3 à 5 minutes).
   Si besoin : *Compiler l'APK → Run workflow*.
4. Cliquez sur l'exécution terminée, puis téléchargez **MonBudget-apk** en bas de la page (un zip contenant `app-debug.apk`).
5. Copiez l'APK sur le téléphone et ouvrez-le. Android demandera d'autoriser l'installation depuis cette source
   (Paramètres → Applications → accès spécial → installer des applis inconnues).

## Ou avec Android Studio

*File → Open* sur ce dossier, attendre la synchronisation, puis *Build → Build APK(s)*.
L'APK est dans `app/build/outputs/apk/debug/`.

## Mises à jour

La clé de signature (`app/debug.keystore`) est fixe : une nouvelle version s'installe par-dessus l'ancienne
sans perdre les données. Conservez ce fichier. L'application elle-même est dans
`app/src/main/assets/index.html`.

Important : désinstaller l'application efface ses données. Faites une sauvegarde (Réglages → Sauvegarde) avant.
