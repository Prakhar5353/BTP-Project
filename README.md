# Thesis Project: Collider-based and Direct Detection Study of Sub-GeV Dark Matter

This repository contains all the Jupyter and Mathematica notebooks, along with FeynRules scripts, used in my undergraduate thesis project—part of my Bachelor's degree in Physics.

## Project Overview

Current dark matter (DM) detection strategies largely focus on weakly interacting massive particles (WIMPs) in the 1–1000 GeV mass range, which are expected to produce nuclear recoil signals detectable by conventional experiments. However, DM candidates lighter than 1 GeV are often overlooked, primarily because their interactions typically fall below the detection thresholds of such experiments.

Despite this, sub-GeV DM remains a well-motivated theoretical possibility, especially given the lack of experimental confirmation for WIMPs. These lighter candidates can still interact with atomic electrons, producing detectable single-electron signals via ionization. Furthermore, they could be produced at electron-positron colliders through interactions mediated by leptophilic operators connecting the DM sector to Standard Model leptons.

This project builds upon earlier work done in a mini-project focused on direct detection, and extends it into collider-based studies of sub-GeV DM.

In the second phase of the project, we developed a collider-based framework using leptophilic effective operators to simulate sub-GeV DM production through mono-photon signatures at electron-positron colliders. The relevant interactions were implemented in **FeynRules** and exported to **MadGraph** for event generation at chosen center-of-mass energies. We analyzed both the DM signal and the dominant Standard Model background process, namely electron-positron to neutrino-antineutrino plus photon. Simulated event distributions were compared with theoretical expectations, and a simple neural network was trained to explore signal-background separation using key kinematic variables.

## Repository Structure

### 1. Matrix Element Calculation
- **File**: `matrix_element.nb` (Mathematica Notebook)  
- **Description**: Calculates the squared matrix element for a key process using helicity amplitude methods, which offer a more computationally manageable approach than conventional trace techniques.

### 2. Collider Detection Computations
- **File**: `collider_notebook.ipynb`  
- **Description**: Performs basic calculations and plots for cross-sections relevant to both signal and background processes.

### 3. Direct Detection Computations
- **File**: `directdetection.ipynb`  
- **Description**: Contains calculations related to the direct detection of sub-GeV DM via electron recoil. This notebook builds upon techniques from an earlier mini-project, exploring the theoretical viability of detecting such particles in low-threshold electron recoil experiments.

### 4. Model Implementation
- **Folder**: `DM_0/`  
- **Contents**: FeynRules scripts for implementing custom DM-SM interaction operators.  
- **Purpose**: Generates **UFO (Universal FeynRules Output)** files for use in MadGraph to simulate collider events.

### 5. Data Analysis and Neural Network Training
- **Folder**: `Data_analysis/`  
- **Contents**: Jupyter Notebooks for:
  - Analyzing signal and background data generated in MadGraph.
  - Plotting key observables using histograms.
  - Training a basic artificial neural network to distinguish signal from background based on kinematic features.

## Skills and Tools

Throughout this project, I gained experience with:

- **FeynRules** – for implementing effective field theory models and exporting to MadGraph.
- **MadGraph5_aMC@NLO** – for event generation based on custom interaction models.
- **Mathematica** – for matrix element calculations using helicity amplitude techniques.
- **Python & Jupyter** – for data analysis, visualization, and neural network training using libraries like NumPy, Matplotlib, and PyTorch.
