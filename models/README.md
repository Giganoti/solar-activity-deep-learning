# Models

This folder documents the deep learning models explored in the Master's Thesis project.

The project compared two neural network architectures for the prediction of extreme solar activity: a one-dimensional Convolutional Neural Network and a Long Short-Term Memory network. Both models were applied to two different prediction tasks: solar flare prediction and coronal mass ejection prediction.

## 1D Convolutional Neural Network

The 1D CNN was used to detect local temporal patterns in satellite time-series data.

In the solar flare prediction task, the model analysed the evolution of X-ray flux before relevant flare events. This approach was useful because solar flares often show detectable radiative patterns shortly before the event.

For the CME prediction task, the same type of architecture was tested using magnetic parameters from active solar regions. However, the results were more limited, suggesting that the available input variables did not contain enough information to fully describe the physical processes involved in CME formation.

## LSTM network

The LSTM model was used to capture sequential dependencies in the data.

This architecture is especially useful for time-series problems because it can learn from the temporal evolution of the input variables. In this project, the LSTM was applied to both flare and CME prediction tasks in order to compare its performance with the 1D CNN.

For solar flare prediction, the LSTM achieved promising results, confirming that the temporal behaviour of the X-ray flux contains useful predictive information.

## Model comparison

The results showed a clear difference between the two prediction problems.

Solar flare prediction achieved better performance, suggesting that X-ray flux data provide a strong signal before flare events. In contrast, CME prediction was more difficult, probably because CMEs depend on larger-scale coronal dynamics that are not fully captured by the magnetic parameters used in the model.

## Notes

Trained model files are not included in this repository. This folder is intended to document the architectures and modelling approach used in the project.

Future versions of the repository may include simplified model examples or clean training scripts.
