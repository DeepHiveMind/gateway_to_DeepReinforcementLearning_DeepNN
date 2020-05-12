Speech Recognition has seen a tremendous improvement in the last 5 years.


# Taxonomy of Speech & Audio domain
* wav file 
[ Audio file container. We use .wav file to read audio as mp3 cannot be read as .txt file. ]

* librosa / pyaudio libraries 
[python libraries to read/transform/process audio files such as .wav]

* Sampling Rate 

* Mono Audio- 1 source of signal. we convert stereo audio to mono audio using Librosa library.

* Fourier Transform 
[It is a tool which allows us to convert our time domain signal into the frequency domain. A signal in the frequency domain requires much less computational space for storage.]

* Mel-frequency cepstral coefficients (MFCCs)
[MFCC is a representation of the short-term power spectrum of a sound, which in simple terms represents the shape of the vocal tract. Our voice/sound is dependent on the shape of our vocal tract including tongue, teeth etc. If we can determine this shape accurately, we can recognize the word/character being said.] 

* Spectrograms
[Spectrograms are another way of representing the audio signal. Spectrograms convey 3-dimensional information in 2 dimensions (2D spectrograms). On the x-axis is time and on the y-axis is frequency. The amplitude of a particular frequency at a particular time is represented as the color intensity at that point.]

* Stochastic Gradient Descent with Restarts (SGDR)
[SGDR uses CosineAnnealing as learning rate annealing technique to train the model. Learning rate is reduced at every iteration (not epoch) of gradient descent and after completion of a cycle, the learning rate is reset i.e set to the initial learning rate. This helps in achieving better generalization. The idea is, if the model is at local minima where a slight change in parameters changes the loss very much, then it is not a good local minimum. By resetting the learning rate, we allow the model to find better local minima in the search space.]

* Snapshot Ensembling
[It is a technique used along with SGDR. The basic idea of ensembling is to train more than one model for a specific task and average out their predictions. Most of the models give different predictions for the same input. So if one model gives the wrong prediction, another model gives the correct prediction.]
