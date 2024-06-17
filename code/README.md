
# Lösungen inverser Probleme: Entfaltung von Energiespektren mit neuronalen Netzen in DSEA

## Bachelorarbeit von Samuel Haefs
Abgabetermin: 30. August 2022

## Betreuer
Tim Ruhe  
Karolin Hymon  
Leonora Kardum

## Datensatz
* Quelle: /net/big-tank/POOL/users/lkardum/new_mc_binning.csv
* Daten wurden in MC Simulation generiert
* beinhaltet 98 Features + 1 Label (Neutrino-Energie)
* 13 Millionen Events

## INFO zu den Jupyter Notebooks
Zum Entfalten des Energiespektrums wird das zugrundeliegende Problem als Klassifikationsproblem betrachtet.
Dazu wird die Energie der Neutrinos diskretisiert.
Die resultierenden Energieklassen stellen die Zielvariable ***y*** dar.

Modelle:
* ***DSEA_NN***: Neuronale Netze in DSEA
* ***DSEA_Random_Forest***: Random Forest in DSEA
* ***NN_"FEATURE"***: reine Klassifikation mit einem neuronalen Netz (mit kummulierten Wahrscheinlichkeiten)

Verschiedene Auswahl von Features:
* ***FeatureList***: Liste mit Feature-Namen die mir gegeben wurde
* ***FeatureImportance***: Features die sich bei Untersuchung der FeatureImportance (siehe ***feature_selection***) als nützlich herausgestellt haben.

Die Bins wurden verschieden generiert:
* ***logBins***: logarithmisch skaliert (default)
* ***equalBins***: Bins gleicher Höhe, dementsprechend wurden die Bin-Grenzen angepasst


# Autor
Samuel Haefs  
[samuel.haefs@tu-dortmund.de](samuel.haefs@tu-dortmund.de)

# Referenzen
[DSEA](https://github.com/mirkobunse/CherenkovDeconvolution.py)  
[Tensorflow](https://www.tensorflow.org/)