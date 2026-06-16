# Deep Learning for Extreme Solar Activity Prediction

This repository presents my Master's Thesis project in Artificial Intelligence, focused on the prediction of extreme solar activity using satellite observations and deep learning models.

The project combines space physics, time-series analysis and neural networks to study two major solar phenomena: solar flares and coronal mass ejections (CMEs). Both events are relevant in the context of space weather, since intense solar activity can affect satellites, communications, GPS systems and electrical infrastructure on Earth.

## Project overview

The main objective of the project was to explore whether deep learning models can detect useful patterns before extreme solar events. The study was divided into two prediction tasks.

The first task focused on solar flare prediction using X-ray flux data from GOES-18. In this case, the models aimed to identify temporal patterns before relevant flare events.

The second task focused on CME prediction using magnetic parameters from SDO/HMI-SHARP, combined with CME event information from SOHO/LASCO. This task was more challenging, since CMEs depend on large-scale coronal dynamics that are not always fully captured by photospheric magnetic variables.

## Data sources

The analysis was based on public satellite observations and catalogues from different space missions.

* **GOES-18** was used to obtain X-ray flux data for solar flare prediction.
* **SDO/HMI-SHARP** provided magnetic parameters from active solar regions.
* **SOHO/LASCO** was used as a reference source for CME event information.

Raw datasets are not included in this repository. The aim of the repository is to document the methodology, models, results and interpretation of the project.

## Methodology

The workflow included data collection, temporal alignment, preprocessing, normalization and event labelling. After preparing the datasets, prediction windows and thresholds were defined in order to train supervised deep learning models.

Two neural network architectures were evaluated: a one-dimensional Convolutional Neural Network and a Long Short-Term Memory network. The 1D CNN was used to identify local temporal patterns in the input series, while the LSTM was used to capture sequential dependencies before solar events.

Both architectures were applied to the flare prediction task and to the CME prediction task, allowing a comparison between the two types of solar phenomena.

## Results

The results were clearly different depending on the phenomenon studied.

For solar flare prediction, both models showed promising performance. The CNN and LSTM models were able to identify relevant patterns in the X-ray flux before flare events, suggesting that this type of signal contains useful predictive information.

For CME prediction, the performance was more limited. This result is also scientifically meaningful, since it suggests that CME forecasting requires additional physical context and probably the integration of coronal observations or image-based data, rather than relying mainly on photospheric magnetic parameters.

## Repository structure

The repository is organized into the following sections:

* [`report/`](report/)
  Contains the final Master's Thesis report.

* [`notebooks/`](notebooks/)
  Reserved for exploratory analysis, model experiments or future reproducibility notebooks.

* [`src/`](src/)
  Reserved for Python scripts related to preprocessing, model training and evaluation.

* [`figures/`](figures/)
  Includes selected figures from the project, such as data visualizations, model results and performance comparisons.

* [`data/`](data/)
  Describes the satellite data sources used in the project and explains why raw datasets are not included.

* [`models/`](models/)
  Documents the neural network architectures explored in the project.

## Skills demonstrated

This project demonstrates the application of artificial intelligence to a scientific problem involving real satellite data. It includes time-series preprocessing, binary classification, deep learning model design, evaluation with metrics such as precision, recall and AUC, and scientific interpretation of model performance.

It also reflects the connection between my background in Physics and my training in Artificial Intelligence, applying machine learning methods to a problem related to space weather and solar activity.

## Future improvements

Future work could focus on making the analysis more reproducible through clean notebooks and scripts, expanding the dataset, and integrating additional data sources such as coronal images. Another relevant improvement would be the use of explainability techniques to better understand which patterns the models are learning before each solar event.
