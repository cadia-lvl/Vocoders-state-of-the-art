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

