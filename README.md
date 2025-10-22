# One-Shot RLVR Evaluation

This repository contains an evaluation implementation of the [One-Shot-RLVR](https://github.com/ypwang61/One-Shot-RLVR) project by ypwang61.

## Overview

This project attempts to recreate and evaluate the One-Shot RLVR (Reinforcement Learning from Visual Representations) model. Due to computational resource constraints, full model training was not feasible. Instead, this repository focuses on **evaluating the pre-trained model** provided by the original authors and analyzing the results.

## Project Structure

The repository contains three main files:

1. **Model Evaluation Notebook** - Loads the pre-trained model from Hugging Face and runs evaluation
2. **Results CSV** - Contains the model's responses saved during evaluation
3. **Results Analysis Notebook** - Extracts and analyzes results from the CSV file

## Workflow

```
1. Load pre-trained model from Hugging Face
   ↓
2. Run evaluation and save responses to CSV
   ↓
3. Extract and analyze results from CSV
```

## Setup

### Prerequisites

```bash
pip install torch transformers datasets pandas numpy
```

### Files Description

- `evaluation.ipynb` - Main evaluation script that:
  - Loads the pre-trained One-Shot RLVR model from Hugging Face
  - Runs inference on the evaluation dataset
  - Saves model responses to CSV format

- `responses.csv` - Contains:
  - Model predictions
  - Ground truth labels
  - Evaluation metrics
  - Additional metadata from the evaluation run

- `extract_results.ipynb` - Post-processing script that:
  - Reads the evaluation CSV
  - Computes final metrics
  - Generates visualizations and analysis

## Usage

### 1. Run Evaluation

Open and run `evaluation.ipynb`:
- This will load the pre-trained model from Hugging Face
- Execute evaluation on the test dataset
- Save results to `responses.csv`

### 2. Analyze Results

Open and run `extract_results.ipynb`:
- Processes the saved CSV file
- Extracts relevant metrics
- Provides analysis and visualizations

## Limitations

- **Training**: Full model training was not performed due to computational resource limitations
- **Evaluation Only**: This repository focuses solely on evaluation using the authors' pre-trained checkpoint
- **Pre-trained Model**: All results are based on the official pre-trained model from Hugging Face

## Original Repository

This work is based on:
- **Repository**: [ypwang61/One-Shot-RLVR](https://github.com/ypwang61/One-Shot-RLVR)
- **Pre-trained Model**: Available on Hugging Face (link in evaluation notebook)

## Acknowledgments

- Original authors of One-Shot-RLVR for providing the pre-trained model
- Hugging Face for model hosting infrastructure

## License

Please refer to the original [One-Shot-RLVR repository](https://github.com/ypwang61/One-Shot-RLVR) for licensing information.

## Citation

If you use this evaluation code or the original One-Shot-RLVR model, please cite the original work:



## Contact

For questions about this evaluation implementation, please open an issue in this repository.

For questions about the original One-Shot-RLVR model, please refer to the [original repository](https://github.com/ypwang61/One-Shot-RLVR).
