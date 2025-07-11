# PoseGaze-AHP Dataset Creation Code

## Overview
This repository contains the code used to create the PoseGaze-AHP dataset - the first publicly available 3D dataset integrating head pose and gaze movement data for AI-driven diagnosis of ocular-induced abnormal head posture (AHP).

## Repository Contents
- **Data Extraction using Claude.ipynb**: LLM-based iterative extraction of clinical data from medical literature using Claude 3.5 Sonnet
- **Ocular Dataset Simulation.ipynb**: 3D head pose and gaze generation using the Neural Head Avatar framework
- **README.md**: This documentation

## Methodology Overview
1. **Literature Collection**: Systematic collection of 148 medical research papers on ocular conditions and AHP
2. **LLM Extraction**: Structured clinical data extraction using Claude 3.5 Sonnet with three prompting strategies
3. **Data Processing**: Standardization and imputation of extracted clinical information
4. **3D Generation**: Transformation into 3D head pose and gaze representations using NHA framework

## Dependencies
- Python 3.8+
- anthropic package (version 0.49.0) for Claude API
- Neural Head Avatar framework (see below)
- Standard data processing libraries (pandas, numpy, etc.)

## Neural Head Avatar Framework
This project utilizes the Neural Head Avatar (NHA) framework for 3D head generation:
- **Original Repository**: https://github.com/philgras/neural-head-avatars/tree/main
- **Setup**: Follow the installation instructions in the original NHA repository

## Usage

### 1. Data Extraction
```bash
# Configure Claude API key
# Run the data extraction notebook
jupyter notebook "Data Extraction using Claude.ipynb"
