# 🫁 Détection des Maladies Pulmonaires par Deep Learning

## 📌 Description du projet
Ce projet vise à concevoir et déployer un **système intelligent d’aide au diagnostic médical** capable de détecter automatiquement les principales maladies pulmonaires à partir de **radiographies thoraciques (X-Ray)**.

Le système repose sur des **réseaux de neurones convolutifs (CNN)** et plus précisément sur l’architecture **DenseNet121**, sélectionnée pour ses performances supérieures en classification multi-classes.

Les pathologies détectées sont :
- ✅ Poumon sain (Normal)
- 🦠 Pneumonie bactérienne
- 🧬 Pneumonie virale (incluant COVID-19)

Une **interface web interactive** a été développée avec **Streamlit** afin de permettre une utilisation simple et rapide du modèle.

---

## 🎯 Objectifs
- Automatiser l’analyse des radiographies pulmonaires
- Aider les radiologues à la prise de décision
- Réduire le temps de diagnostic
- Atteindre une précision supérieure à 80 %

---

## 🧠 Approche Méthodologique
Le projet suit la méthodologie **CRISP-DM** :
1. Compréhension du problème médical
2. Compréhension et analyse des données
3. Préparation des données
4. Modélisation
5. Évaluation
6. Déploiement

---

## 🗂️ Dataset
- **Nombre total d’images** : 11 712
- **Types d’images** : Radiographies thoraciques (X-Ray)
- **Répartition** :
  - 70 % entraînement
  - 15 % validation
  - 15 % test

---

## 🏗️ Architecture du Modèle
- **Modèles testés** :
  - ResNet50
  - DenseNet121 ✅ (modèle retenu)

- **Techniques utilisées** :
  - Transfer Learning
  - Data Augmentation
  - Dropout pour éviter l’overfitting
  - Optimiseur : Adam
  - Fonction de perte : Categorical Crossentropy

---

## 📊 Résultats
| Modèle        | Précision globale |
|--------------|------------------|
| ResNet50     | 72.15 %          |
| DenseNet121  | **85.37 %** ✅   |

### Performances clés (DenseNet121) :
- 🔍 **Rappel pneumonie bactérienne** : **99.2 %**
- ⚡ Inférence quasi instantanée
- ❌ Très peu de faux négatifs (critère crucial en médecine)

---

## 💻 Interface Utilisateur
L’application a été développée avec **Streamlit** et permet :
- Le chargement d’une radiographie
- L’affichage de la classe prédite
- La visualisation des probabilités associées à chaque classe

---

## 🛠️ Technologies utilisées
- **Python**
- **TensorFlow / Keras**
- **Streamlit**
- **NumPy / Matplotlib**
- **OpenCV**
- **GPU NVIDIA GTX 1650 Super**

---

## ⚙️ Installation et Exécution

### 1️⃣ Cloner le projet
```bash
git clone https://github.com/votre-username/detection-maladies-pulmonaires.git
cd detection-maladies-pulmonaires
