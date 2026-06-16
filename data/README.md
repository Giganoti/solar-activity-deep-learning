# Data

Raw satellite datasets are not included in this repository.

This project was based on public observations and catalogues from space missions used to study solar activity. The data were used to build two prediction tasks: solar flare prediction and coronal mass ejection prediction.

## Main data sources

The analysis used three main sources of satellite data:

* **GOES-18**
  Used to obtain X-ray flux time-series data for solar flare prediction. These data were especially relevant for detecting temporal patterns before M- and X-class flare events.

* **SDO/HMI-SHARP**
  Used to obtain magnetic parameters from active solar regions. These variables were used as input features for the CME prediction task.

* **SOHO/LASCO**
  Used as a reference catalogue for coronal mass ejection events, allowing the construction of labels for the CME prediction problem.

## Data preparation

The workflow involved collecting the data, aligning the different sources in time, cleaning the records, normalizing the variables and defining event labels. Prediction windows and thresholds were then created so that the models could learn from the temporal behaviour before solar events.

## Why the raw data are not included

The original datasets are not uploaded to this repository because they come from external scientific missions and may contain large files. The purpose of this repository is to document the methodology, models, figures and results developed during the Master's Thesis project.

## Notes

Future versions of this repository may include small sample datasets or simplified examples to make parts of the workflow easier to reproduce.
