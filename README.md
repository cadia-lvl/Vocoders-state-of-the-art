# Vocoders-state-of-the-art

This github page contains all the Vocoding methods we tested for both Icelandic and English.

- Mixed-Excitation-Based Vocoders 
  - Channel vocoder
    - STRAIGHT
    - WORLD 
  - Phase vocoder 
    - Griffin-Lim
    - MagPhase
- Neural Vocoders
  - WaveNet
  - LPCNet
- Glottal-Excitation-Based Vocoders 
- Sinusoidal Vocoders 

![taxonomy](./img/newtaxonomy.png)

_Coprehensive taxonomy of speech coders based on different vocoding schemes._

## STRAIGHT

__Abstract__

STRAIGHT, a speech analysis, modification synthesis system, is an extension of the classical channel VOCODER that exploits the advantages of progress in information processing technologies and a new conceptualization of the role of repetitive structures in speech sounds. This review outlines historical backgrounds, architecture, underlying principles, and representative applications of STRAIGHT.

Source:
[STRAIGHT exploitation of the other aspect of VOCODER Perceptually isomorphic decomposition of speech sounds](https://www.researchgate.net/publication/228741024_STRAIGHT_exploitation_of_the_other_aspect_of_VOCODER_Perceptually_isomorphic_decomposition_of_speech_sounds)

Code:
[STRAIGHT, written in MATLAB](https://github.com/HidekiKawahara/legacy_STRAIGHT)


## WORLD

__Abstract__

A vocoder-based speech synthesis system, named WORLD, was developed in an effort to improve the sound quality of real-time applications using speech. Speech analysis, manipulation, and synthesis on the basis of vocoders are used in various kinds of speech research. Although several high-quality speech synthesis systems have been developed, real-time processing has been difficult with them because of their high computational costs. This new speech synthesis system has not only sound quality but also quick processing. It consists of three analysis algorithms and one synthesis algorithm proposed in our previous research. The effectiveness of the system was evaluated by comparing its output with against natural speech including consonants. Its processing speed was also compared with those of conventional systems. The results showed that WORLD was superior to the other systems in terms of both sound quality and processing speed. In particular, it was over ten times faster than the conventional systems, and the real time factor (RTF) indicated that it was fast enough for real-time processing.

Source:
[WORLD: A Vocoder-Based High-Quality Speech Synthesis System for Real-Time Applications](https://www.researchgate.net/publication/304671740_WORLD_A_Vocoder-Based_High-Quality_Speech_Synthesis_System_for_Real-Time_Applications)

Code:
[WORLD, written in python](https://github.com/JeremyCCHsu/Python-Wrapper-for-World-Vocoder)


## Griffin-Lim

__Abstract__

In this paper, we present an algorithm to estimate a signal from its modified short-time Fourier transform (STFT). This algorithm is computationally simple and is obtained by minimizing the mean squared error between the STFT of the estimated signal and the modified STFT. Using this algorithm, we also develop an iterative algorithm to estimate a signal from its modified STFT magnitude. The iterative algorithm is shown to decrease, in each iteration, the mean squared error between the STFT magnitude of the estimated signal and the modified STFT magnitude. The major computation involved in the iterative algorithm is the discrete Fourier transform (DFT) computation, and the algorithm appears to be real-time implementable with current hardware technology. The algorithm developed in this paper has been applied to the time-scale modification of speech. The resulting system generates very high-quality speech, and appears to be better in performance than any existing method.

Source:
[Signal Estimation from Modified Short-Time Fourier Transform](https://ieeexplore.ieee.org/document/1164317)

Code:
[Griffin-Lim, written in python](https://github.com/bkvogel/griffin_lim)

## MagPhase

__Abstract__

Missing

Source:
[Direct Modelling of Magnitude and Phase Spectra for Statistical Parametric Speech Synthesis](https://www.researchgate.net/publication/319185348_Direct_Modelling_of_Magnitude_and_Phase_Spectra_for_Statistical_Parametric_Speech_Synthesis)

Code:
[MagPhase, written in python](https://github.com/CSTR-Edinburgh/magphase)

## WaveNet

__Abstract__

This paper introduces WaveNet, a deep neural network for generating raw audio waveforms. The model is fully probabilistic and autoregressive, with the predictive distribution for each audio sample conditioned on all previous ones; nonetheless we show that it can be efficiently trained on data with tens of thousands of samples per second of audio. When applied to text-to-speech, it yields state-of-the-art performance, with human listeners rating it as significantly more natural sounding than the best parametric and concatenative systems for both English and Mandarin. A single WaveNet can capture the characteristics of many different speakers with equal fidelity, and can switch between them by conditioning on the speaker identity. When trained to model music, we find that it generates novel and often highly realistic musical fragments. We also show that it can be employed as a discriminative model, returning promising results for phoneme recognition.

Source:
[WaveNet: A Generative Model for Raw Audio](https://arxiv.org/abs/1609.03499)

Code:
[WaveNet, written in python and PyTorch](https://github.com/r9y9/wavenet_vocoder)

## LPCNet

__Abstract__

Neural speech synthesis models have recently demonstrated the ability to synthesize high quality speech for text-to-speech and compression applications. These new models often require powerful GPUs to achieve real-time operation, so being able to reduce their complexity would open the way for many new applications. We propose LPCNet, a WaveRNN variant that combines linear prediction with recurrent neural networks to significantly improve the efficiency of speech synthesis. We demonstrate that LPCNet can achieve significantly higher quality than WaveRNN for the same network size and that high quality LPCNet speech synthesis is achievable with a complexity under 3 GFLOPS. This makes it easier to deploy neural synthesis applications on lower-power devices, such as embedded systems and mobile phones.

Source:
[LPCNet: Improving Neural Speech Synthesis Through Linear Prediction](https://arxiv.org/abs/1810.11846)

Code:
[LPCNet, written in C, python and Keras](https://github.com/mozilla/LPCNet)
