# Welcome to Classically Punk
## Task
The Task was to find a library that "reads" music files. Also, to identify features inside the music files that will be used to separate a collection of music files into different music genres.
Therefore, the task is to build an application in Python that automatically classifies different musical genres from an audio snippet.

## Description
I used the following functions on the dataset provided:
def feature_extractor(path, frame_size=2048, hop_length=126, num_frames=10): It was used to extract audio features from audio files in a specified directory using 'librosa.load()'  and returned the Pandas DataFrame containing the aggregated feature values for all audio files in the specified directory("C:/Users/bukol/OneDrive/Documents/genres")
def plot_waveform(path, num_rows=2, num_cols=5):it was used to visualize the raw waveform of audio files in a specified directory('/content/drive/MyDrive/MUSIC') using 'os.walk()', 'librosa.load()', and 'librosa.display.waveshow() for all the 10 music genres 
def plot_spectrograms(path, num_rows=2, num_cols=5):It took the directory path(('/content/drive/MyDrive/MUSIC') as input, reads audio files from different subdirectories in that path, and then plots the spectrograms of the audio signals in a grid of subplots for each of these features extracted(mfcc', 'chroma_stft', and 'Chroma_energy')
def plot_zero_crossing_rate(path, num_rows=2, num_cols=5):It was used to plot the zero crossing rate spectrogram on the corresponding subplot , with the genre label as the title.
def count_zero_crossings(path):It was used to count the total number of zero crossings in the audio files located in a specific directory.
def plot_spectral_centroid(path, num_rows=2, num_cols=5):It was used to plot the spectral centroid for the audio files located in a specific directory to identify differences in the brightness or timbre of the audio signals across genres.
def plot_spectral_rolloff(path, num_rows=2, num_cols=5):It was used to plot the spectral rolloff for the audio files located in a specific directory to identify differences in the overall brightness or spectral distribution of the audio signals across genres.
def prepare_data(X,y,test_size=0.1, validation_size=0.1): It was used to split the input data and labels into training, validation, and test sets for machine learning model
The model was trained and evaluated using model = Sequential(), compiled by Adam optimizer and was trained for 100 epochs

## Installation
There was no need for any installation as it can be run on local machine using Jupyter notebook and other necessary dependencies like Librosa, scikit-learn, numpy, pandas

## Usage
The code was run on a jupyter notebook whose http address can be gotten by running this in the terminal:
jupyter notebook
then the jupyter address can be followed after inserting 'web' and the password 'qwasar' inputed
Run 'pip install Librosa on the terminal
Run 'pip install -U scikit-learn'

### The Core Team
Bukola Veronica Oladele(veronica_b)


<span><i>Made at <a href='https://qwasar.io'>Qwasar SV -- Software Engineering School</a></i></span>
<span><img alt='Qwasar SV -- Software Engineering School's Logo' src='https://storage.googleapis.com/qwasar-public/qwasar-logo_50x50.png' width='20px'></span>
