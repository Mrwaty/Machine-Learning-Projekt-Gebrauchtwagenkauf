# Machine Learning Projekt: Gebrauchtwagenkauf

Dieses Projekt beschäftigt sich mit der Klassifikation von Fehlkäufen bei Gebrauchtwagenauktionen mithilfe von Machine Learning.

## Projektstruktur

Die Dokumentation ist in sechs Abschnitte unterteilt:

1. [Einleitung](docs/1.Einleitung.pdf)  
2. [Explorative Datenanalyse (EDA)](docs/2.EDA.pdf)  
3. [Outlier-Erkennung](docs/3.Outliers.pdf)  
4. [Datenvorbereitung](docs/4.Data_Preperation.pdf)  
5. [Modellierung](docs/5.Modeling.pdf)  
6. [Interpretation & Ergebnisse](docs/6.Interpretation.pdf)

# Einleitung

Ein US-amerikanischer Gebrauchtwagenhändler kauft Fahrzeuge über Onlineauktionen. Einige Fahrzeuge weisen schwerwiegende Mängel auf („Montagsautos“) und verursachen hohe Folgekosten.

# Explorative Datenanalyse (EDA)

- Datensatz: 65.620 Fahrzeuge, 33 Merkmale  
- Zielvariable: `IsBadBuy` (unausgeglichen: ca. 12 % Fehlkäufe)

**Analyseschritte:**
- Visualisierung der Zielverteilung  
- Heatmap der Korrelationen

# Outliers

- Ausreißeranalyse mit Boxplots und RANSAC  

# Data Preparation (zur Modellierung)

- Train-Test Split
- Data Imputation
- OneHotEncoding für kategorische Merkmale
- SMOTE zur Ausbalancierung der Zielvariable 

# Modeling

**Verwendete Modelle:**
- Logistische Regression  
- Random Forest  
- Entscheidungsbaum  
- Ensemble-Modell (VotingClassifier)

**Techniken:**
 
- GridSearchCV zur Hyperparameteroptimierung  
- PCA zur Dimensionsreduktion
- Feature Selection

# Interpretation

- Aufbau der finalen Datenpipeline
- Speicherung die vorhergesagten Werte für 'IsBadBuy' (Zielvariable) in einer CSV-Datei


## Zielsetzung

Ziel war es, ein Modell zu entwickeln, das auf Basis von Fahrzeugdaten erkennt, ob ein Auto ein Fehlkauf darstellt („Montagsauto“).

## Technologien

- Python (pandas, scikit-learn, matplotlib, seaborn)
- Jupyter Notebook
- Git & GitHub


