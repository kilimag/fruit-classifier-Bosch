

# Fruchtklassifikations-Projekt
## Projektübersicht
Dieses Projekt zielt darauf ab, ein Modell zu entwickeln, das verschiedene Fruchttypen (z. B. Äpfel, Bananen, Trauben) basierend auf ihren Eigenschaften Gewicht, Farbe und Größe klassifiziert. Dabei werden zwei Ansätze evaluiert:

1. Logistische Regression
2. Entscheidungsbaum

Die Analyse umfasst die Datenaufbereitung, explorative Datenanalyse, Modelltraining und Hyperparameter-Tuning. Die Modelle werden anhand verschiedener Metriken wie Genauigkeit, F1-Score und ROC-AUC verglichen.

# Projektstruktur
Das Projekt ist in mehrere Ordner unterteilt, um die Organisation und Nachvollziehbarkeit zu gewährleisten:

📂 data

      ├── fruit_data.xlsx              #Rohdatensatz
      ├── fruit_data_cleaned.xlsx      #Bereinigte und aufbereitete Daten
📂 models
      
      ├── model_training.ipynb         # Notebook mit Modelltraining und Evaluierung

📂 notebooks

      ├── data_preparation.ipynb       # Datenaufbereitung und Bereinigung
      ├── exploratory_analysis.ipynb   # Explorative Datenanalyse
   
📄 README.md               

# Datenbeschreibung
Die Daten enthalten die folgenden Variablen:

**fruit_type**: Zielvariable (Fruchttyp: Apple, Banana, Grape).

**weight**: Gewicht der Frucht (numerisch).

**size**: Größe der Frucht (kategorisch: Tiny, Small, Medium, Large).

**color**: Farbe der Frucht (kategorisch: Yellow, Pale Yellow, Red, Purple, Pink, Green, Creamy White, Black).

Die Daten wurden bereinigt und nach fehlenden Werten geprüft. Details dazu finden Sie im Notebook data_preparation.ipynb.

# Durchgeführte Schritte
1. Datenvorbereitung
      - Entfernen von fehlenden oder fehlerhaften Werten.
      - Transformation kategorischer Variablen in numerische Werte.
      - Optional: Skalierung numerischer Variablen.
2. Explorative Datenanalyse
      - Untersuchung der Verteilung der Daten.
      - Visualisierungen wie Boxplots, Heatmaps und Histogramme.
      - Beispiel: Gewichtsunterschiede zwischen Fruchttypen.
3. Modelltraining
      - Training eines Entscheidungsbaums und einer logistischen Regression.
      - Anwendung von Hyperparameter-Tuning (Grid Search) zur Optimierung des Entscheidungsbaums.
      - Vergleich der Modellleistungen anhand:
            - Genauigkeit
            - F1-Score
            - ROC-AUC
5. Ergebnisse

      - Die logistische Regression zeigte eine Genauigkeit von 93% und schnitt insgesamt besser ab.

      - Der Entscheidungsbaum erreichte die gleiche Genauigkeit, jedoch mit einer geringeren AUC.

# Anleitung zur Reproduktion
1. Repository klonen

            git clone https://github.com/kilimag/fruit-classifier-Bosch
            cd fruit-classifier-Bosch
2. Python-Umgebung einrichten
Installieren Sie die benötigten Abhängigkeiten:

            pip install -r requirements.txt
3. Notebooks ausführen

- Beginnen Sie mit data_preparation.ipynb, um die Daten aufzubereiten.
- Führen Sie exploratory_analysis.ipynb aus, um die explorative Analyse zu sehen.
- Führen Sie model_training.ipynb aus, um die Modelle zu trainieren und zu evaluieren.
4. Ergebnisse überprüfen

- Modelle und Ergebnisse sind im Ordner Models gespeichert.
- Visualisierungen und Metriken sind in den Notebooks dokumentiert.
