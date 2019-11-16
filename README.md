# genre-classification-pop-prediction
The objective of this project is to tackle the problem of automatic genre classification of
tracks, along with prediction of a song’s popularity. An approach using Machine Learning techniques for the tasks
of predicting the popularity of a song, and also to classify the song into genres. Automatic Genre Classification of songs can be achieved, and before a song hits the
charts, it’s popularity can be predicted, so that recommendation can be done.

Requirements : 
1. Operating System : Linux based Operating System with Python version >=3.5 
2. Librosa Module : For audio extraction
3. NumPy : Numerical Python module for data manipulation
4. Pandas : Data Structures
5. Keras : Machine learning module built on top of TensorFlow
6. Sklearn : Machine Learning module scikit-learn
7. Genre Classification : Audio data obtained from UCI Machine Learning Repository (8000 tracks , 30 seconds each)
8. Popularity Prediction : Data obtained from Spotify’s Web API (features of each
audio track)

Genre Classification : In our approach, we use the python librosa module to extract features of a song from it’s spectrogram. The features we obtain are :
1. Zero Crossing Rate
2. Spectral Centroid
3. Spectral Rolloff
4. Mel-Frequency Cepstral Coefficient
5. Chroma Freq.
6. Tonnetz
These features are fed into a classifier which outputs one amonst 8 genres.

Popularity Prediction : Using Spotify Web API, we obtain features of a track such as it’s danceability, energy etc. These are fed into a linear regressor for baseline performace, and then to an MLP classifier.
