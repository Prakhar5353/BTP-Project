# Thesis Project: Collider-based Search for Sub-GeV Dark Matter via Mono-photon Signatures

This repository stores all the Jupyter and Mathematica notebooks, as well as the FeynRules scripts, used in my undergraduate thesis project—part of my Bachelor’s degree in Physics.

## Project Overview

We developed a collider-based framework using leptophilic effective operators to model sub-GeV Dark Matter (DM) production through mono-photon signatures at \(e^+e^-\) colliders. The interactions were implemented in **FeynRules** and exported to **MadGraph** for event generation at relevant center-of-mass energies.

Both signal and background processes were analyzed, with a focus on a dominant Standard Model neutrino background. Simulated event distributions were compared with theoretical differential cross-sections across various key kinematic variables. To explore the potential for signal-background discrimination, a simple artificial neural network was trained using these variables.

## Repository Structure

### 1. Matrix Element Calculation
- **File**: `matrix_element.nb` (Mathematica Notebook)  
- **Description**: Calculates the matrix element squared for a key process. Due to the complexity of the spinor algebra, conventional trace methods were not sufficient. Helicity amplitude methods were used instead, which allow the problem to be handled computationally using vectors and matrices.

### 2. Cross-Section Computations
- **File**: `boltzmann_proper.ipynb`  
- **Description**: Contains basic calculations and plots of various cross-sections relevant to the DM production and background processes.

### 3. Model Implementation
- **Folder**: `DM_0/`  
- **Contents**: FeynRules scripts for implementing new DM-SM interaction operators.  
- **Purpose**: Generates **UFO (Universal FeynRules Output)** files, which are compatible with MadGraph for event generation.

### 4. Data Analysis and Neural Network Training
- **Folder**: `Data_analysis/`  
- **Contents**: Jupyter Notebooks that:
  - Analyze signal and background events generated using MadGraph.
  - Create histograms for various observables.
  - Train a simple artificial neural network to test signal-background separation using kinematic features.

## Skills and Tools

Throughout this project, I gained experience with:

- **FeynRules** – for implementing effective field theory operators and generating UFO models.
- **MadGraph5_aMC@NLO** – for simulating collider events based on custom interaction models.
- **Mathematica** – for matrix element calculations using helicity amplitude techniques.
- **Python & Jupyter Notebooks** – for data analysis, visualization, and machine learning using libraries like NumPy, Matplotlib, and PyTorch.
