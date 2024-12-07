

# Fruchtklassifikations-Projekt
## Projektübersicht
Dieses Projekt zielt darauf ab, ein Modell zu entwickeln, das verschiedene Fruchttypen (z. B. Äpfel, Bananen, Trauben) basierend auf ihren Eigenschaften wie Gewicht und Größe klassifiziert. Dabei werden zwei Ansätze evaluiert:

1. Logistische Regression
2. Entscheidungsbaum

Die Analyse umfasst die Datenaufbereitung, explorative Datenanalyse, Modelltraining und Hyperparameter-Tuning. Die Modelle werden anhand verschiedener Metriken wie Genauigkeit, F1-Score und ROC-AUC verglichen.

# Projektstruktur
Das Projekt ist in mehrere Ordner unterteilt, um die Organisation und Nachvollziehbarkeit zu gewährleisten:

📂 Data ├── raw_data.csv # Rohdatensatz ├── cleaned_data.csv # Bereinigte und aufbereitete Daten 📂 Models ├── model_training.ipynb # Notebook mit Modelltraining und Evaluierung ├── decision_tree.pkl # Gespeichertes Entscheidungsbaum-Modell ├── logistic_regression.pkl # Gespeichertes logistisches Regressionsmodell 📂 Notebooks ├── data_preparation.ipynb # Datenaufbereitung und Bereinigung ├── exploratory_analysis.ipynb # Explorative Datenanalyse 📄 README.md # Diese Dokumentation

# Datenbeschreibung
Die Daten enthalten die folgenden Variablen:

**fruit_type**: Zielvariable (Fruchttyp: Apple, Banana, Grape).

**weight**: Gewicht der Frucht (numerisch).

**size**: Größe der Frucht (kategorisch: Tiny, Small, Medium, Large).

**color**: Farbe der Frucht (kategorisch: Yellow, Red, Purple, Pink, Green, Creamy White, Black).

Die Daten wurden bereinigt und nach fehlenden Werten geprüft. Details dazu finden Sie im Notebook data_preparation.ipynb.

