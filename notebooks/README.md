# Notebooks

This folder contains the main Google Colab notebooks developed during the Master's Thesis project.

The notebooks document the experimental workflow used for the prediction of extreme solar activity with deep learning models. They include data loading, preprocessing, event labelling, model training and evaluation for two prediction tasks: solar flares and coronal mass ejections.

## Notebooks

* `01_solar_flare_prediction_goes18.ipynb`
  Notebook focused on solar flare prediction using GOES-18 X-ray flux data. It includes the preparation of the X-ray time series, flare event labelling, model training and evaluation of deep learning approaches.

* `02_cme_prediction_sdo_sharp_soho_lasco.ipynb`
  Notebook focused on coronal mass ejection prediction using SDO/HMI-SHARP magnetic parameters and SOHO/LASCO CME event information. It explores the use of deep learning models for a more complex prediction task.

## Notes

The raw satellite datasets are not included in this repository, so the notebooks may require path adaptations or access to the corresponding public data sources before being executed.

These notebooks reflect the experimental workflow developed during the Master's Thesis. They are included to document the applied modelling process and the connection between satellite data, preprocessing, neural networks and model evaluation.
