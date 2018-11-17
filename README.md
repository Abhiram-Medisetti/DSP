# DSP TRANSFORMS

What is my audio signal?
While taking an audio signal('audio.wav') as input I have truncated the length of data to nearest exponent of 2.
When reading the data from the audio signal, it should be of the type 1D array. If your data is of type 2D array, then you need to take the 1st colomn of the data.

How can you see whether compression took place or not?
I have transformed the audio signal into 3 domains. They are Discrete Fourier Transform, Discrete Cosine Transform and Haar Transform. In each domain I have added zeros (while storing the data in transformed domain, I left out the zeros and stored the other coefficients), and calculated inverse transforms which ideally should lead to the original sequence( if no data is lost).
As I have stored the coefficients in a text file, we can see that the size of the text file reduces as the number of zeros increases.

How to know what extent of data is corrupted?
I have calculated the error of the calculated signal and actual signal for various number of zeros(compression) and stored them in a list.The error increases as the number of zeros increases. The extent of error for a particular number of zeros in more for Fourier Transform than Cosine Transform.
