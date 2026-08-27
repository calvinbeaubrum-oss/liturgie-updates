# Liturgie — canal de mise à jour

**Nox Studio — développé par Promethe.** Contact : junsam713@gmail.com

Ce dépôt est le **canal public de mise à jour** de l'application Android « Liturgie ».
Il ne contient **que** les fichiers nécessaires à la mise à jour in-app :

| Fichier | Rôle |
|---|---|
| `manifest.json` | Dernière version publiée (versionCode, URL APK, SHA-256) |
| `versions.json` | Historique complet des versions téléchargeables |

Le **code source n'est pas ici** (dépôt privé). Aucune donnée personnelle n'est collectée.

## Comment l'app utilise ce dépôt

1. L'app lit `manifest.json` (au lancement + 1×/jour, Wi-Fi uniquement par défaut).
2. Si une version plus récente existe : notification → tu choisis « J'adopte » ou « Plus tard ».
3. L'APK est téléchargé puis son intégrité **SHA-256 vérifiée** avant installation.
4. Paramètres → Mise à jour → **Choisir une version** : liste complète via `versions.json`.

Aucune mise à jour ne s'installe sans ton accord explicite.
