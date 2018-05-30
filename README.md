# Speech-recognition

The project is closely related to Automatic Speech Recognition except that instead of recognizing the continuous speech constituting of many different words and sentences, we will be recognizing a small set of words and label remaining as unknown or silence. The training and test data contains wave files of nearly one second long each one uttering a word, noise or just silence. 
The datasets required to train this project are provided by Google as part of a kaggle speech recognition challenge (kaggle). 

## Usage:

Download the train and test data from the below link.
https://www.kaggle.com/c/tensorflow-speech-recognition-challenge/data

Maintain the folder structure as 
ipython notebook
data/train etc.

create a folder called silence in data/train/audio and run DataExploration.ipynb to genrate few silence data samples from _background_noise_ wav files.

remove _background_noise_ folder from data/train/audio and run Speech_recognition_Submit.ipynb notebook.


## Improvement:
 
1. The dimensionality of features is huge and try using PCA to remove some dimensions of negligible variance before passing it to the model for training. 
2. Though the MFCC features are state of the art in speech recognition based on the literature, we should try other features like raw wave, fft, log mel features etc and combinations of different features as well. 
3. We should try using few other neural network layers for mfcc features and see how the model performs. Some of them might include: a. Convolution LSTM. b. VGGbn19. c. InceptionResnetV2. d. Densenet201 etc. 
4. I should try other models like XGBoost (LGBM implementation, as it is computationally effective), random forest kind of ensemble models and see how they perform on this Multi-classification problem. 
5. I should either setup or rent GPU to run these models as these will take days if I were to run on normal CPU. I need to make use floydhub, paperspace or vectordash in future. 
6. I believe, experimenting all these options with proper computational power will definitely enhance my final benchmark model. 
7. Listen to mislabeled samples in validation set. 
8. Data augmentation: Add heavy noise augmentation while keeping noise vs signal ratio below 2. 
 

## References:

**Boiler Plate** : https://www.kaggle.com/davids1992/speech-representation-and-data-exploration 

**MFCC** : https://librosa.github.io/librosa/generated/librosa.feature.mfcc.html

**Keras** : https://keras.io/layers/recurrent/#lstm
https://ideasforeversite.wordpress.com/2018/03/18/automatic-speech-recognition/
http://practicalcryptography.com/miscellaneous/machine-learning/guide-mel-frequency-cepstral-coefficients-mfccs/ 

**Voice Activity Detection** : https://pypi.python.org/pypi/webrtcvad , https://github.com/wiseman/py-webrtcvad/blob/master/example.py,
https://github.com/marsbroshok/VAD-python, https://github.com/marsbroshok/VAD-python/blob/master/detectVoiceInWave.py



