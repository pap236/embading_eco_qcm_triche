# embading_eco_qcm_triche

## Analyse sémantique des questions à choix multiples en économie avec SentenceTransformers

---

### Description

Ce projet propose une méthode automatisée d’analyse des questionnaires à choix multiples (QCM) en économie, basée sur des modèles d’embeddings sémantiques.  
En utilisant la bibliothèque **SentenceTransformers**, le système calcule la similarité entre chaque question et ses différentes options de réponse pour :

- Identifier l’option la plus proche sémantiquement,
- Ajouter au dataset des colonnes indiquant le score de similarité maximal,
- Ajouter l’index de la meilleure réponse prédite,
- Faciliter l’évaluation automatique des QCM complexes.

Ce projet est idéal pour les enseignants, chercheurs ou développeurs intéressés par le traitement automatique du langage naturel (NLP) appliqué à l’évaluation pédagogique.

---

### Fonctionnalités

- Chargement et traitement d’un fichier CSV contenant questions et options
- Calcul des embeddings avec le modèle `all-MiniLM-L6-v2` (ou tout autre modèle compatible)
- Calcul des similarités cosinus entre la question et chaque option
- Ajout des colonnes de résultats au dataset
- Export vers un nouveau fichier CSV enrichi

---

### Prérequis

- Python 3.7 ou plus
- Bibliothèques Python :
  - pandas
  - sentence-transformers
  - torch (installé automatiquement avec sentence-transformers)

```bash
pip install pandas sentence-transformers
