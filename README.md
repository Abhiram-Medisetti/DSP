# DSP TRANSFORMS

What is my audio signal?
While taking an audio signal('audio.wav') as input I have truncated the length of data to nearest exponent of 2.
When reading the data from the audio signal, it should be of the type 1D array. If your data is of type 2D array, then you need to take the 1st colomn of the data.

How can you see whether compression took place or not?
I have also uploaded outputs folder.
I have transformed the audio signal into 3 domains. They are Discrete Fourier Transform, Discrete Cosine Transform and Haar Transform. I have truncated the transform data based on number of zeros and uploaded the transform data in a text file.You can see that the size of text file keeps on decreasing as the number of zeros increases. 
This text file is then read to calculate the inverse transform and i have used that to obtain the reverted signal from original.

How to know what extent of data is corrupted?
I have calculated the error of the calculated signal and actual signal for various number of zeros(compression) and stored them in a list.The error increases as the number of zeros increases. The extent of error for a particular number of zeros in more for Fourier Transform than Cosine Transform.
