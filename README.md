# Speech-recognition

https://www.kaggle.com/c/tensorflow-speech-recognition-challenge

Predicting words using LSTM neural network

Put your data folder in the same folder as that of your notebook.

You can find data required for this project in below link
https://www.kaggle.com/c/tensorflow-speech-recognition-challenge/data 

Some of the Blog posts followed:
1. https://ideasforeversite.wordpress.com/2018/03/18/automatic-speech-recognition/
2. http://practicalcryptography.com/miscellaneous/machine-learning/guide-mel-frequency-cepstral-coefficients-mfccs/ 
3. Voice Activity Detection : https://pypi.python.org/pypi/webrtcvad , https://github.com/wiseman/py-webrtcvad/blob/master/example.py

https://github.com/marsbroshok/VAD-python

https://github.com/marsbroshok/VAD-python/blob/master/detectVoiceInWave.py

Libraries used:

1. For extracting MFCC features : https://librosa.github.io/librosa/generated/librosa.feature.mfcc.html
2. Keras : https://keras.io/layers/recurrent/#lstm

To do:

1. Add silence detection.
2. Scale it for more words in future.
3. Try delta mfcc features.
4. Try PCA on features.

Boiler plate:
https://www.kaggle.com/davids1992/speech-representation-and-data-exploration 



