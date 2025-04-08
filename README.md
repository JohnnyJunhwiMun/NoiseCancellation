# Statistical Signal Processing: Noise Cancellation with FIR Filtering


## Table of Contents
- [Introduction](#introduction)
- [Technical Background](#technical-background)
- [Implementation Details](#implementation-details)
  - [Signal Processing Approach](#signal-processing-approach)
  - [Technical Setup](#technical-setup)
- [Key Features](#key-features)
- [Usage Instructions](#usage-instructions)
- [Results](#results)
- [Future Improvements](#future-improvements)

---

## Introduction

This project implements a noise cancellation system using Wiener filtering techniques to recover clean audio signals from noisy recordings. It addresses a common challenge in RF communications where transmitted signals are corrupted by additive Gaussian noise.

---

## Technical Background

The received signal is modeled as:

```math
x(n) = d(n) + v(n)
```
where:

- `x(n)`: The received signal
- `d(n)`: The original signal of interest
- `v(n)`: Additive Gaussian noise (statistically uncorrelated with `d(n)`)


---
## Implementation Details

### Signal Processing Approach

The system employs Wiener filtering to design a Finite Impulse Response (FIR) filter that optimally estimates and recovers the original signal. Key aspects include:

- **Signal Modeling**: All signals are treated as discrete-time and real-valued.
- **Noise Characteristics**: Noise is modeled as Gaussian and uncorrelated with the original signal.
- **Filter Design**: An FIR filter, denoted as W(z), is implemented based on the statistical properties of the signal and noise.

### Technical Setup

The project utilizes the following resources and libraries:

- **Data Files**:
  - Three test recordings (`notes_xxx.mat`)
  - Background noise recording (`noise.mat`)

- **Python Libraries**:
  - **NumPy**: For numerical computations.
  - **Matplotlib**: For data visualization.
  - **SciPy**: For signal processing functions.
  - **Sounddevice**: For audio playback.

---

## Key Features

- **Statistical Signal Processing**: Implements an effective noise cancellation algorithm using statistical methods.
- **RF Communication Scenario**: Addresses real-world noise challenges in RF communications.
- **Wiener Filtering**: Leverages optimal filtering techniques to recover the original audio signal.
- **Discrete-Time Processing**: Focuses on digital processing of audio signals.
- **Audio Signal Recovery**: Demonstrates practical recovery of clean audio from noisy recordings.

---

## Usage Instructions

1. **Prepare the Data**:  
   Ensure that the test recordings (`notes_xxx.mat`) and background noise recording (`noise.mat`) are available.

2. **Process the Signals**:  
   Use the provided Python scripts to load the audio files and apply the Wiener filter to the signals.

3. **Evaluate the Results**:  
   - Compare the original and recovered signals through visual plots and audio playback.
   - Assess the effectiveness of the noise cancellation process using the provided evaluation tools.

---

## Results

The implementation showcases:

- **Effective Noise Reduction**: Significantly minimizes the impact of Gaussian noise in RF communications.
- **Clean Signal Recovery**: Successfully recovers the original audio signal with high fidelity.
- **Practical Application**: Demonstrates the application of statistical signal processing in a real-world scenario.

---

## Future Improvements

Potential enhancements for future iterations include:

- **Real-Time Noise Cancellation**: Develop capabilities for real-time processing of audio signals.
- **Adaptive Filtering**: Integrate adaptive filtering techniques to better handle dynamic noise environments.
- **Enhanced Algorithms**: Explore advanced signal recovery methods for more robust performance.
- **Diverse Noise Scenarios**: Extend testing to include various noise sources beyond Gaussian, improving system versatility.


