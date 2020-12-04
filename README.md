# Phase-retrieval

School project in association with the ONERA the French Aerospace Lab.
The project goal is to test and optimize some phase-retrieval algorithms to perform imagery through scattering media such as skin or fog.

The image of an object taken through a scattering media creates a random Speckle pattern on the camera sensor.
The intensity of the image can be easily retrieved by performing a 2D autocorrelation of the Speckle pattern and then perform a 2D Fourier transform of it according to the Wiegner-Khintchine theorem. 

However, the phase of the image can't be accessed so easily. And it appears that the phase of an image looks like it carries more information than its intensity.
Therefore, some algorithms are needed to retrieve the phase of the image.

I first investigated error reduction algorithm that is a generalization of the Gerchberg–Saxton algorithm to retrieve the phase.
This is an iterative algorithm for retrieving the phase of a pair of light distributions related via a propagating function, here the Fourier transform.

Finally, I investigated a Bispectrum method to retrieve the phase. The Bispectrum or Bispectral density is a mathematical tool to access higher order spectra of a signal (here an image) and possibly retrieve its phase.
