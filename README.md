# DAQS Project — Speech Quality Evaluation (Natural vs. Synthetic)

This project implements the **DAQS (Disagreement-Aware Quality Score)** for evaluating the quality of speech synthesis systems compared to natural speech.

## Project Details
- **Student**: Qammar Mehmood
- **Email**: qamarmehmood2001@gmail.com
- **Roll Number**: 26I-7800
- **Topic**: T6 — Speech Quality Evaluation: Natural vs. Synthetic

## Repository Structure
- `26I-7800_notebook.ipynb`: The main research and implementation notebook.
- `requirements.txt`: Python dependencies.
- `.gitignore`: Configured to exclude large datasets and temporary files.

## Setup Instructions

### 1. Prerequisites
- **Python 3.10+**
- **FFmpeg**: Required by Whisper for audio processing.
  - On Windows, you can install it via `pip install imageio-ffmpeg` (the notebook handles the path injection automatically).

### 2. Dataset
This project uses the **LJSpeech-1.1** dataset.
1. Download it from [here](https://keithito.com/LJ-Speech-Dataset/).
2. Extract it into the root directory of this project so the folder is named `LJSpeech-1.1/`.

### 3. Environment Setup
Create a virtual environment and install the dependencies:
```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
```

### 4. Running the Notebook
Open `26I-7800_notebook.ipynb` in VS Code or Jupyter and run the cells in order.
> **Note**: The first run of DNSMOS and Whisper will download their respective neural models (approx. 500MB+).

## Key Features
- **MCD, PESQ, UTMOS, DNSMOS, WER**: Implementation of 5 diverse speech metrics.
- **DAQS Formula**: A composite score that penalizes model disagreement.
- **Statistical Testing**: Significance testing (Wilcoxon) and Ablation studies.
- **Visualization**: Detailed correlation and distribution plots.
