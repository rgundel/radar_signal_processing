# Radar Signal Processing Project
## Sub-project: Radar Range Equation

* **Author**: Dr. Ronny Guendel
* **Date**: 26. May '24  
* **Website**: [rgundel.github.io](https://rgundel.github.io/)
* **Code language**: MATLAB, Python
* **Environment**: MATLAB, Jupyter Notebook

## Project Overview

This repository contains code for various radar range equations and signal-to-noise ratio (SNR) calculations. The content is organized into different sections covering fundamental concepts and practical implementations in radar signal processing.

## Content

### MATLAB Files
- **radar_signal_processing.m**: MATLAB code for calculating received power, noise power, and SNR.

### Python Files
- **radar_signal_processing.ipynb**: Jupyter Notebook with Python code for calculating received power, noise power, and SNR.

## Example Calculations

### Received Power of a Target
The received power ($P_r$) is calculated using the radar range equation:
$P_r = \frac{P_t G_t G_r \lambda^2 \sigma}{(4\pi)^3 R^4}$

### Signal-to-Noise Ratio (SNR)
The SNR is calculated as:
$\text{SNR} = \frac{P_r}{P_n}$

Converted to dB:
$SNR_{dB} = 10 \log_{10}(SNR)$

### SNR in dB as Summation Equation
$SNR_{dB} = P_{t_{dB}} + G_{t_{dB}} + G_{r_{dB}} + 20 \log_{10}(\lambda) + 10 \log_{10}(\sigma) - factor_{dB} - 40 \log_{10}(R) - k_{dB} - T_{0_{dB}} - F_{dB} - B_{dB}$


Where:
- $P_{t_{\text{dB}}} = 10 \log_{10}(P_t)$
- $G_{t_{\text{dB}}} = 10 \log_{10}(G_t)$
- $G_{r_{\text{dB}}} = 10 \log_{10}(G_r)$
- $20 \log_{10}(\lambda)$ converts the wavelength term to dB
- $10 \log_{10}(\sigma)$ converts the radar cross-section to dB
- $\text{factor}_{\text{dB}} = 10 \log_{10}((4 \pi)^3)$
- $40 \log_{10}(R)$ converts the range term to dB
- $k_{\text{dB}} = 10 \log_{10}(k)$
- $T_{0_{\text{dB}}} = 10 \log_{10}(T_0)$
- $F_{\text{dB}} = 10 \log_{10}(F)$
- $B_{\text{dB}} = 10 \log_{10}(B)$

## Usage

1. Clone the repository:
```sh
git clone https://github.com/rgundel/radar_signal_processing.git
