# 🦆 QUACKEMS 3-Input Test Board

> Quantitative Charge Kinetic Energy Mass Sensor — Front-End Test System  
> Designed and assembled by **Emma Stensland**

## 🧠 Overview

The **3-Input Test Board** analyzes charge pulses from the **W1 Silicon Strip Detector** for the **QUACKEMS** instrument.  
It converts detector charge pulses into shaped Gaussian voltage pulses for further signal analysis and detector characterization.

## 🔬 Theory of Operation

- The **W1 Silicon Strip Detector** acts as a reverse-biased diode.  
  Charged particles crossing the depletion zone produce ionized charge carriers that drift to the electrodes, forming a charge pulse.  
- The **test board** conditions this signal through:
  - A **charge-sensitive preamplifier** that integrates the charge and produces a decaying voltage pulse.
  - A **Gaussian shaper** that converts the preamp’s exponential tail into a smooth, bell-shaped waveform.  
- The system is enclosed in a custom **grounded metal enclosure** functioning as a **Faraday cage** to minimize noise.

## 🧭 Design Overview

The PCB is a **four-layer design**:

| Layer | Function |
|--------|-----------|
| 1 | Ground plane, bias, and surface-mount signal routing |
| 2 | Shielded preamp I/O lines |
| 3 | Dedicated ground plane |
| 4 | Power routing for preamp and shaper stages |

## 📚 References

- [Cremat Inc. — Preamplifier & Shaper Modules](https://www.cremat.com/)  
- [CERN: Introduction to Silicon Strip Detectors (PDF)](https://indico.cern.ch/event/124392/contributions/1339904/attachments/74582/106976/IntroSilicon.pdf)  
- CR-110-R2.2 Datasheet  
- CR-200-R2.1 Datasheet  
- W1 300 µm Detector Documentation  
