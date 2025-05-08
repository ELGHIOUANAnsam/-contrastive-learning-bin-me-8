Contrastive Learning Lab 
📝 Projet réalisé par : (Binôme_8)
- ELGHIOUAN Ansam
- MAGHNOUJ Ayoub

📝Encadré par : Pr. MAHMOUDI Abdelhak

🔹 Description du projet :

Ce projet fait partie du Lab sur l’Apprentissage Contrastif, où nous explorons les principes du contrastive learning et son application en deep learning.
L’objectif est d’entraîner un modèle capable de comparer et distinguer des images en se basant sur leurs représentations dans un espace d’embeddings.
Nous utilisons le dataset CIFAR-10, qui est téléchargé automatiquement via torchvision.datasets.CIFAR10.

💡 Aucune manipulation manuelle des fichiers n'est requise, PyTorch gère directement le téléchargement et l’accès aux données.

📌 Toutes les étapes du projet peuvent être exécutées directement depuis le Notebook Jupyter ou Google Colab, sans nécessiter de scripts externes.


🔹 Structure du Projet  

Ce projet est organisé de manière à faciliter la navigation et l'exécution des différentes étapes.

📂 Jupyter Notebook

-  → Contient tout le code du projet, incluant l'entraînement et l'évaluation du modèle contrastif.


📂 Documentation

- README.md → Fichier expliquant le projet, son fonctionnement, et les instructions pour l’exécuter.


📂 Vidéo de Présentation

- video/presentation_lab.mp4 → Vidéo de présentation directement disponible dans le repo.


🔹 Vidéo de Présentation
	🎥 Vidéo disponible dans le repo : presentation_lab.mp4
 
	⏳ Durée : 
 
	📌 Contenu de la vidéo :
	- Explication de l’environnement de développement
 	- Présentation du code et de l’apprentissage contrastif
	- Résultats obtenus et analyse

🔹 Installation & Prérequis
Avant de lancer le projet, assurez-vous d’avoir :
✅ Python 3.10+
✅ Les dépendances listées dans requirements.txt

🔹 Installation des dépendances depuis requirements.txt :
    pip install -r requirements.txt
*(Cela permet d’installer toutes les bibliothèques nécessaires en une seule commande).

🔹 Explication du Modèle
Nous avons implémenté un modèle contrastif basé sur un réseau de neurones convolutif (CNN), entraîné à distinguer les images similaires et différentes.
📌 Principales étapes :
🔹 Prétraitement des images → Normalisation et transformation des données CIFAR-10.
🔹 Création d’embeddings → Passage des images dans le modèle pour obtenir des représentations vectorielles.
🔹 Calcul de la distance → Comparaison des paires d’images et définition de la similarité.
🔹 Optimisation du modèle → Utilisation de Adam comme optimiseur et de la perte contrastive pour affiner l’apprentissage.

🔹 Entraînement du Modèle
Le modèle est entraîné sur l’ensemble d’apprentissage de CIFAR-10, où il apprend à différencier les images similaires et différentes.

📌 Toutes les étapes d'entraînement sont exécutées directement dans le Notebook Jupyter.

✅ Optimisation avec Adam pour ajuster les poids du modèle.

✅ Utilisation de la perte contrastive pour affiner la distinction entre les images.

✅ Affichage dynamique avec tqdm pour suivre la progression de l’apprentissage.

🔹 Évaluation du Modèle
Après l'entraînement, le modèle est testé sur l’ensemble de test de CIFAR-10 pour mesurer sa capacité à généraliser.
📌 Toutes les étapes d'évaluation sont exécutées directement dans le Notebook Jupyter.
✅ Précision obtenue sur les données de test CIFAR-10 : varie généralement entre **82% et 88.66%** -et par fois encor plus -, 
    en fonction du nombre d’epochs réalisés avant interruption. Plus l’entraînement dure, plus la précision augmente.
✅ Affichage amélioré avec la barre de progression (tqdm) pour un suivi dynamique.
✅ Le modèle démontre une bonne capacité à distinguer les images similaires et différentes.


Remerciements
Nous remercions notre professeur pour son encadrement et accompagnement ainsi que les différentes ressources qui nous ont aidés à approfondir notre compréhension de l’apprentissage contrastif.
💡 Ce projet nous a permis d’explorer un concept clé en deep learning et de le mettre en application avec un modèle performant. 
