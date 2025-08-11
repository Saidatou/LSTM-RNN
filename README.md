Titre du projet
LSTM-RNN – Prédiction de mots avec un réseau récurrent à mémoire long terme (LSTM)

Description
Ce projet implémente un modèle de réseau de neurones récurrent (LSTM) pour effectuer de la prédiction de texte, à partir d’un corpus (ici, le texte de "Hamlet"). Le codage est en Python avec une interface via app.py et un pipeline exploratoire dans un notebook (experiemnts.ipynb).

Contenu du dépôt
app.py : script principal pour utiliser ou interagir avec le modèle entraîné.

experiemnts.ipynb : notebook d'exploration, préparation des données, entraînement, visualisations, etc.

hamlet.txt : corpus source utilisé pour l'entraînement (extrait de Hamlet).

next_word_lstm.h5 & next_word_lstm_model_with_early_stopping.h5 : modèles entraînés sauvegardés (non-stop et avec early stopping).

tokenizer.pickle : fichier de tokenisation pour convertir le texte en séquences numériques utilisables par le modèle.

requirements.txt : liste des dépendances Python nécessaires.

Fonctionnement général
Chargement des données — Lecture du fichier texte et construction du corpus textuel à partir duquel les séquences sont générées.

Prétraitement — Tokenisation du texte, conversion en séquences d’indices à l’aide du tokenizer enregistré.

Entraînement du modèle — Un réseau LSTM est entraîné à prédire le mot suivant dans une séquence. L’entraînement peut inclure l’early stopping pour éviter le surapprentissage.

Utilisation du modèle entraîné — app.py permet de charger le modèle et le tokenizer, de générer des prédictions à partir d’une entrée textuelle, etc.

Exploration et visualisation — Le notebook experiemnts.ipynb documente le processus d’entraînement, les métriques, et fournit une visualisation des résultats.


Usage
Entraîner le modèle : exécuter le notebook experiemnts.ipynb pour l’entraînement depuis les données brutes.

Prédiction interactive : lancer python app.py pour générer un mot à partir d’une séquence donnée.

avantage du projet : 
Ce projet permet de comprendre les mécanismes de base d’un modèle LSTM appliqué à la génération de texte — préparation des données, tokenisation, construction du modèle, entraînement, évaluation et utilisation pratique. C’est un outil idéal pour apprendre à manipuler des RNN/LSTM de manière intuitive et concrète.