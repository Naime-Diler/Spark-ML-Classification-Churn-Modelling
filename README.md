Im Projekt **„Spark Machine Learning: Churn Modelling“** wird Spark Machine Learning eingesetzt, um Kundenabwanderungen vorherzusagen. Die wesentlichen Schritte sind:

**Datenvorbereitung:** Der Datensatz wird aus einer CSV-Datei geladen und in einem DataFrame gespeichert. Die Datentypen werden überprüft, und der Datensatz wird im Speicher gehalten, um die Verarbeitung zu beschleunigen.

**Datenverarbeitung:** Kategorische und numerische Merkmale werden identifiziert und verarbeitet. Kategorische Spalten werden aufbereitet, indem führende und nachfolgende Leerzeichen entfernt werden. Für die One-Hot-Codierung ausgewählte Spalten werden mit `StringIndexer` in numerische Indizes umgewandelt. Ein `OneHotEncoder` wird verwendet, um diese Indizes in One-Hot-Features zu kodieren.

**Modelltraining:** Ein Gradient-Boosted Tree Classifier wird innerhalb einer Spark-Pipeline trainiert, um Kundenabwanderungen zu klassifizieren. Die Pipeline umfasst die Schritte der Datenumwandlung, Feature-Extraktion und Skalierung.

**Evaluation:** Die Modellleistung wird mit dem Area Under ROC (AUC)-Wert bewertet, um die Genauigkeit der Vorhersagen zu messen.

Dieses Projekt veranschaulicht, wie Spark ML zur effizienten Verarbeitung und Modellierung von Daten verwendet wird, um präzise Klassifikationen und Vorhersagen zu ermöglichen.
