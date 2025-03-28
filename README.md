# ECG Signal Processing Project

## Overview
This project is part of **ECEN 3301 - Biomedical Signals and Systems** and focuses on processing **electrocardiogram (ECG) signals**. The goal is to design digital filters, automate heart rate analysis, and detect **ventricular arrhythmias** using **MATLAB**.

### Objectives:
- **Data Acquisition**: Understanding ECG signal characteristics.
- **Signal Conditioning**: Removing noise using bandpass filters.
- **Heart Rate Analysis**: Detecting and plotting heart rate trends.
- **Arrhythmia Detection**: Identifying abnormal heart rhythms.

## Repository Structure
```
ECG-Signal-Processing/
│── data/                     # Raw and processed data files
│   ├── normal.mat
│   ├── n_422.mat
│   ├── n_421.mat
│── scripts/                  # MATLAB scripts and live scripts
│   ├── data_acquisition.mlx  # Task 1-3: Data loading & block diagram
│   ├── signal_processing.mlx  # Task 4-7: Noise filtering & conditioning
│   ├── heart_rate_analysis.mlx  # Task 8-11: Heart rate measurement
│   ├── arrhythmia_detection.mlx  # Task 12-15: Arrhythmia detection
│── results/                  # Output plots, processed signals
│   ├── filtered_signals/
│   ├── heart_rate_plots/
│   ├── arrhythmia_results/
│── docs/                     # Report & documentation
│   ├── report.pdf            # Final report
│   ├── README.md             # Project overview and instructions
│── .gitignore                # Ignore unnecessary files (e.g., MATLAB cache)
│── LICENSE                   # License (MIT recommended)
│── README.md                 # Overview of the project
```

## Getting Started
### Prerequisites
- **MATLAB (Recommended R2022a or later)**
- Signal Processing Toolbox (optional but helpful)

### Setup Instructions
1. **Clone the repository:**
   ```bash
   git clone https://github.com/brendanharrington/ECG-Signal-Processing.git
   cd ECG-Signal-Processing
   ```
2. **Open MATLAB and navigate to the repository:**
   ```matlab
   cd 'path/to/ECG-Signal-Processing'
   ```
3. **Load ECG data:**
   ```matlab
   load('data/normal.mat');
   ```
4. **Run a script:**
   ```matlab
   run('scripts/signal_processing.mlx');
   ```

## Project Breakdown
### 1️⃣ Data Acquisition
- Reads and loads ECG signals.
- Constructs a block diagram for the acquisition process.

### 2️⃣ Signal Conditioning
- Implements bandpass filters to remove noise.
- Evaluates time and frequency domain responses.

### 3️⃣ Heart Rate Analysis
- Automates heart rate measurement.
- Uses Fourier Transform and peak detection.

### 4️⃣ Arrhythmia Detection
- Analyzes ventricular flutter and fibrillation.
- Implements an automated classification algorithm.

## Results
- Filtered ECG signals stored in `results/filtered_signals/`
- Heart rate trend plots saved in `results/heart_rate_plots/`
- Arrhythmia detection results stored in `results/arrhythmia_results/`

