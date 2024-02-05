Harmful Brain Activity Detection Classification - Classify seizures and other patterns of harmful brain activity in critically ill patients

Dataset from Harvard Medical School (Kaggle Competition)
https://www.kaggle.com/competitions/hms-harmful-brain-activity-classification/overview

The goal of this competition is to detect and classify seizures and other types of harmful brain activity in electroencephalography (EEG) data.
Predictions are evaluated on the Kullback Liebler divergence between the predicted probability and the observed target.

The content of the notebook:
  - Converting Kaggle provided spectrograms (parquet format) to numpy arrays
  - Manual converting EEGs to spectrograms, so more information is fed to the network.
  - Splitting datasets to train and validation sets, reshaping them accordingly to the spectrogram duration and frequency.
  - Training the pretrained model (EfficientNet V2)


Joblib was used for pipelining the process of reading and cinverting thousands EEGs and spectrograms.
Librosa library was used for converting EEGs to spectrograms.

