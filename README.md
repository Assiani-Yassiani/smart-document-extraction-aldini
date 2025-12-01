# Document Data Extractor - Aldini France

Système intelligent d'extraction automatique de données à partir de documents administratifs et commerciaux. Solution développée pour optimiser le traitement des documents KBIS, factures et autres documents officiels.

## 🎯 Objectif

Automatiser l'extraction et la structuration des informations clés présentes dans les documents PDF (KBIS, factures, documents administratifs) afin d'éliminer la saisie manuelle et réduire les erreurs.

## 🔄 Pipeline du Système

### 1. Réception du Document
Upload du document PDF via une API REST sécurisée. Le système accepte les documents scannés et natifs, avec validation automatique du format et de la taille.

### 2. Reconnaissance Optique de Caractères (OCR)
Analyse du document PDF et extraction du texte complet grâce à des modèles de computer vision spécialisés. Traitement optimisé pour gérer les documents de qualité variable.

### 3. Extraction Intelligente des Entités
Identification et extraction des champs clés du document à l'aide d'un modèle de traitement du langage naturel (NLP). Le système reconnaît automatiquement les informations structurées et non-structurées.

### 4. Validation et Structuration
Nettoyage et formatage des données extraites. Validation des formats (adresses, codes postaux, numéros SIRET) et structuration en format JSON exploitable.

### 5. Export des Résultats
Génération automatique d'un fichier JSON structuré contenant toutes les informations extraites, prêt à être intégré dans les systèmes d'information existants.

## 📋 Données Extraites

### Documents KBIS
- Dénomination sociale
- Numéro d'identification (SIREN/SIRET)
- Forme juridique
- Capital social
- Adresse complète du siège (rue, code postal, ville)
- Nom des gérants et dirigeants
- Activités principales

### Documents Commerciaux
- Informations entreprise
- Coordonnées complètes
- Données financières
- Contacts clés

## 🛠️ Technologies et Modèles Utilisés

- **OCR (Computer Vision)**: Doctr - Modèle de reconnaissance optique de caractères
- **NLP (Extraction d'Entités)**: GLiNER - Modèle de Named Entity Recognition pour extraction intelligente
- **Backend**: Flask - API REST
- **Traitement de Données**: Python, Regex
- **Format de Sortie**: JSON structuré

## 📊 Performances

- Temps de traitement: 3-5 secondes par document
- Précision d'extraction: >95% sur documents standards
- Formats supportés: PDF (natif et scanné)
- Taille maximum: 16 MB par fichier
- Architecture: API REST scalable



*Projet développé pour Aldini France - Solution d'extraction intelligente de documents*
