# Sécurisation & Administration Active Directory (GPO) 🛡️

Ce projet porte sur l'analyse des besoins, la rédaction d'un cahier des charges et le déploiement concret de stratégies de groupe (GPO) pour sécuriser une infrastructure Windows Server multi-sites (Lyon, Paris, Lille).

## 🚀 Fonctionnalités & Missions
- **Analyse des Risques** : Homogénéisation des configurations hétérogènes et renforcement de la sécurité globale.
- **Durcissement Système (Hardening)** :
    - Désactivation de PowerShell et de l'invite de commande (CMD) pour les utilisateurs standards.
    - Restriction d'accès au Panneau de configuration et blocage des périphériques USB/Bluetooth.
    - Activation de BitLocker pour le chiffrement des lecteurs.
- **Gestion des Services** :
    - Déploiement centralisé des mises à jour via **WSUS**.
    - Mise en place du système de fichiers distribués **DFS** pour la haute disponibilité des données.
    - Configuration forcée de **Firefox ESR** (Proxy, page d'accueil, extensions).
- **Identité Visuelle** : Déploiement automatique de fonds d'écran par site et messages légaux au login.

## 📂 Contenu du dépôt
- `scripts/` : Éventuels scripts d'automatisation.
- `docs/` : Documentation technique et captures d'écran des configurations.
- `JOLIVEL-SAVAGE_Raphael_TP_GPO.pdf` : Rapport complet de mise en œuvre technique.

## 🛠️ Validation du POC
L'application des stratégies a été validée sur une Unité d'Organisation (OU) de test (`POC-GPO`) via les outils de diagnostic natifs :
- `gpupdate /force` pour l'actualisation immédiate.
- `gpresult /h` pour la génération de rapports d'exécution HTML.


**Auteurs :** Raphaël JOLIVEL-SAVAGE & Ethan MÉNOURY
