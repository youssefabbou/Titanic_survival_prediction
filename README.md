# Titanic_survival_prediction


Dieses Projekt verwendet den Titanic-Datensatz, um mithilfe von maschinellem Lernen die Überlebenswahrscheinlichkeit der Passagiere vorherzusagen. Es umfasst die Datenvorbereitung, explorative Datenanalyse (EDA), Feature-Engineering und Modellierung mit einem Random-Forest-Klassifikationsmodell.

## Datenquelle

Der verwendete Datensatz basiert auf den Titanic-Daten, die ursprünglich über Kaggle zur Verfügung gestellt wurden. Die Daten wurden bereinigt, fehlende Werte behandelt und kategorische Variablen in numerische Werte umgewandelt, um sie für die Modellierung vorzubereiten.

## Projektstruktur

1. **Datenbereinigung**:
   - Fehlende Werte wurden entsprechend behandelt.
   - Irrelevante Spalten, wie zum Beispiel die `body`-Spalte, wurden entfernt.

2. **Explorative Datenanalyse (EDA)**:
   - Es wurden Visualisierungen erstellt, um die Überlebensrate in Bezug auf Geschlecht und Passagierklasse zu analysieren.
   - Ergebnisse zeigen, dass Frauen und Passagiere der 1. Klasse eine höhere Überlebensrate haben.

3. **Feature-Engineering**:
   - Kategorische Variablen wie Geschlecht und Einschiffungshafen wurden in numerische Werte umgewandelt (z.B. `sex_male`, `embarked_Q`, `embarked_S`).
   - Die verwendeten Features für das Modell sind: `pclass`, `age`, `sibsp`, `parch`, `fare`, `sex_male`, `embarked_Q`, `embarked_S`.

4. **Modellierung**:
   - Ein Random-Forest-Klassifikationsmodell wurde verwendet, um die Überlebenswahrscheinlichkeit der Passagiere vorherzusagen.
   - Das Modell wurde auf Trainingsdaten trainiert und auf Testdaten evaluiert.

5. **Evaluation**:
   - Das Modell erreicht eine Genauigkeit von 77,48 %.
   - Die Precision und Recall für Überlebende und Nicht-Überlebende waren relativ ausgewogen, was darauf hinweist, dass das Modell gute Vorhersagen für beide Klassen treffen kann.

## Installation und Verwendung

### Voraussetzungen:
- Python 3.x
- Bibliotheken: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

### Schritte zur Ausführung:

1. Repository klonen:
   ```bash
   git clone https://github.com/youssefabbou/titanic-survival-prediction.git
   ```

2. Abhängigkeiten installieren:
   ```bash
   pip install -r requirements.txt
   ```

3. Jupyter Notebook ausführen:
   - Öffne das Jupyter Notebook `Titanic_Analyse.ipynb` und führe die Zellen der Reihe nach aus, um die Analyse und Modellierung zu reproduzieren.

## Ergebnisse

Das Random-Forest-Modell erzielte eine Genauigkeit von **77,48 %** auf den Testdaten. Die Precision und Recall waren relativ ausgewogen, was zeigt, dass das Modell sowohl Überlebende als auch Nicht-Überlebende korrekt vorhersagen kann.

- **Genauigkeit (Accuracy)**: 77,48 %
- **Precision und Recall**: Sowohl für Überlebende als auch für Nicht-Überlebende wurden gute Vorhersagen getroffen.

## Fazit

Dieses Projekt zeigt, wie verschiedene Merkmale von Titanic-Passagieren, wie Geschlecht, Alter und Klasse, die Überlebenswahrscheinlichkeit beeinflussen. Das eingesetzte Random-Forest-Modell hat gute Vorhersageergebnisse geliefert und könnte weiter optimiert werden, indem zusätzliche Features oder komplexere Modelle integriert werden.

## Dateien im Repository

- `Titanic_Analyse.ipynb`: Jupyter Notebook mit der vollständigen Analyse, EDA und Modellierung.
- `bereinigter_titanic_datensatz.csv`: Der bereinigte Titanic-Datensatz, der für die Analyse verwendet wurde.
- `README.md`: Diese Dokumentation.
- `requirements.txt`: Liste der erforderlichen Python-Bibliotheken für das Projekt.
- `README.md`: Diese Dokumentation.
