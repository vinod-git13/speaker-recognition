# speaker-recognition
Context 

Speaker Recognition has always been a cool part to work on in AI.

Content 


This dataset contains speeches of five prominent leaders namely; Benjamin Netanyahu, Jens Stoltenberg, Julia Gillard, Margaret
Tacher and Nelson Mandela which also represents the folder names. Each audio in the folder is a one-second 16000 sample rate PCM encoded.

Originally, the speech for each speaker was a one lengthy audio, I chunked them into one-second each for easier workability. If you combine the chunked audios from 0.wav to 1500.wav, it forms a complete speech of the respective speaker.

A folder called background_noise contains audios that are not speeches but can be found inside and around the speaker environment e.g audience laughing or clapping. It can be mixed with the speech while training.

Acknowledgements

I would like to acknowledge American Rhetoric (online speech bank) for
making the speeches available.

Inspiration

It is somewhat challenging to build small speech recognition models which are very accurate. My goal for this dataset is to develop models that are small enough to be deployed on an mobile device with less compute but at the same time be more accurate. You can
refer to this project to see what have done.

IMPORTED FILES

tensorflow

os

numpy

shutil

keras

After importing necessary libraries,  I arranged the audio and noice.
Then get the list of all noices..then after few lines of code , I splitted noice into chunks of 16,000 steps each.
Data set is generated and noice is added to the data set.
Shuffle to generate random data.
Split into training and validation.
Create datasets,One for training and the other for validation.

Under feature extraction 

Add noise to the training set
Transform audio wave to the frequency domain using `audio_to_fft`.

Modelling is done

Training is done, and epochs are created.

ACCURACY

In the beginning the accuracy is low , as more epochs are executed the accuracy increases
and loss significantly decreases.

PREDICTION

Based on real time ,we are giving the speaker to be predicted , and the model predicts the speaker,based on training data.





