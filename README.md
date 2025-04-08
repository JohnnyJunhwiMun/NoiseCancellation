# Statistical Signal Processing: Noise Cancellation with FIR Filtering

## Project Overview
This project implements a noise cancellation system using Wiener filtering techniques to recover clean audio signals from noisy recordings. The system addresses a common challenge in RF communications where transmitted signals are corrupted by additive Gaussian noise.

## Technical Background
The received signal is modeled as:
```
x(n) = d(n) + v(n)
```
where:
- `x(n)` is the received signal
- `d(n)` is the original signal of interest
- `v(n)` is additive Gaussian noise (statistically uncorrelated with d(n))

## Implementation Details

### Signal Processing Approach
The project uses Wiener filtering to design a Finite Impulse Response (FIR) filter that optimally estimates and recovers the original signal. Key aspects include:

1. **Signal Modeling**: All signals are treated as discrete-time and real-valued
2. **Noise Characteristics**: The noise is modeled as Gaussian and uncorrelated with the signal
3. **Filter Design**: Implementation of FIR filter W(z) based on statistical properties

### Technical Setup
The project includes:
- Three test recordings (`notes_xxx.mat`)
- Background noise recording (`noise.mat`)
- Python implementation using:
  - NumPy for numerical computations
  - Matplotlib for visualization
  - SciPy for signal processing
  - Sounddevice for audio playback

## Key Features
- Statistical signal processing implementation
- Real-world RF communication scenario
- Practical noise cancellation using Wiener filtering
- Discrete-time signal processing
- Audio signal recovery demonstration


## Usage
1. Load the audio files:
   - Test recordings (`notes_xxx.mat`)
   - Background noise (`noise.mat`)
2. Process the signals using the implemented Wiener filter
3. Compare original and recovered signals
4. Play back the results

## Results
The implementation demonstrates:
- Effective noise reduction in RF communications
- Recovery of clean audio signals from noisy recordings
- Practical application of statistical signal processing techniques

## Future Improvements
- Real-time noise cancellation implementation
- Adaptive filtering for dynamic noise environments
- Enhanced signal recovery algorithms
- Integration with different types of noise sources 
