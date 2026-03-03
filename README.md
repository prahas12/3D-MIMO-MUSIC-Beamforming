# 3D MIMO Beamforming using MUSIC Algorithm

## 📡 Project Overview

This project implements a complete 3D Direction of Arrival (DOA)
estimation pipeline using a planar MIMO antenna array.

The system compares classical Bartlett beamforming with the
high-resolution MUSIC (Multiple Signal Classification) algorithm to
demonstrate the resolution advantage of subspace-based methods over
conventional beamforming.

The implementation is modular and structured to reflect a practical
radar signal processing architecture.

------------------------------------------------------------------------

## 🔬 Features

-   Planar 4×4 MIMO array simulation
-   Narrowband signal modeling for multiple targets
-   Sample covariance matrix estimation
-   Eigenvalue decomposition for signal/noise subspace separation
-   2D MUSIC spatial spectrum computation
-   Classical Bartlett beamformer implementation
-   Automatic peak detection for DOA estimation
-   3D spatial spectrum comparison visualization
-   Additional analytical plots:
    -   Top-view heatmap
    -   Azimuth slice
    -   Eigenvalue spectrum

------------------------------------------------------------------------

## 🎯 Key Insight

Classical beamforming produces wider lobes and limited angular
resolution.

MUSIC, based on signal/noise subspace separation, achieves significantly
sharper peaks and superior angular resolution --- particularly when
targets are closely spaced.

The side-by-side comparison clearly illustrates this performance
difference.

------------------------------------------------------------------------

## 🧠 Algorithms Implemented

-   Sample Covariance Matrix Estimation
-   Eigenvalue Decomposition
-   Signal and Noise Subspace Separation
-   Noise Subspace Projection (MUSIC)
-   2D Grid-Based Spatial Spectrum Scanning
-   Bartlett (Conventional) Beamforming
-   Peak Detection for DOA Estimation

------------------------------------------------------------------------

## ⚙️ System Configuration

-   Carrier Frequency: 77 GHz
-   Array Type: 4×4 Planar Rectangular Array
-   Element Spacing: λ/2
-   Number of Targets: 2
-   SNR: 20 dB
-   Scan Grid:
    -   Azimuth: -90° to 90°
    -   Elevation: -30° to 30°

------------------------------------------------------------------------

## 📁 Project Structure
mimo_3d_beamforming\
│
├── config.py               # System & simulation parameters\
├── array_geometry.py       # Planar array coordinate generation\
├── signal_simulator.py     # Target signal modeling & steering vectors\
├── covariance.py           # Sample covariance matrix computation\
├── music_2d.py             # 2D MUSIC spectrum implementation\
├── beamformer.py           # Classical Bartlett beamformer\
├── peak_detection.py       # DOA peak extraction\
├── visualization.py        # 3D & analytical plotting utilities\
├── main.py                 # Pipeline execution entry point\
└── README.md

------------------------------------------------------------------------

## ▶️ How to Run

Install required libraries:

          pip install numpy matplotlib

Run the simulation:

          python main.py

------------------------------------------------------------------------

## 📌 Applications

-   Automotive Radar Signal Processing
-   3D Direction of Arrival Estimation
-   Array Signal Processing Research
-   Subspace-Based Super-Resolution Methods

------------------------------------------------------------------------

## 👨‍💻 Author

Developed as part of advanced exploration in array signal processing and
high-resolution DOA estimation.
