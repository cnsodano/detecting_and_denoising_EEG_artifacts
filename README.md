# detecting_and_denoising_EEG_artifacts
Public repo to demonstrate some code I wrote for a previous project replicating the results of https://ieeexplore.ieee.org/document/10130669. As this was a group project where the replication of the deep neural network which denoised the EEG data included others' code, I post here just the preprocessing pipeline that I wrote myself.


Script separates an uninterrupted stream of brain activity in to segements and mixes eye-blink artifact into those segments with random starting locations and with varying degrees of signal-to-noise ratio. The resulting contaminated data can be used to train a deep neural network to predict where exactly the noise was mixed in, and to compare the result post-denoising to the original, uncontaminated data.
