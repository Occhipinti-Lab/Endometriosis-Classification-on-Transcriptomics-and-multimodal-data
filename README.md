# Endometriosis-Classification-on-Transcriptomics-and-multimodal-data

# Project Setup Guide

This guide will help you set up the project environment, install dependencies, and run Jupyter notebooks with Python 3.10.

---

## 1. Clone the Repository
```bash
git clone https://github.com/Occhipinti-Lab/Endometriosis-Classification-on-Transcriptomics-and-multimodal-data.git
cd Endometriosis-Classification-on-Transcriptomics-and-multimodal-data-main

```
## 2. Create a Virtual Environment (Python 3.10)

which ever machine you're using you need to create a virtual environment to use it by python 3.10. Because some of The scFBApy functions supports only python 3.10.

### Create virtual environment with Python 3.10
python3.10 -m venv venv

### Activate virtual environment
### For Linux/macOS:
source venv/bin/activate
### For Windows (PowerShell):
### venv\Scripts\activate

### Upgrade pip and install dependencies
pip install --upgrade pip
pip install -r requirements.txt

### (If requirements.txt is missing, install Jupyter manually)
### pip install jupyter ipykernel

### Add virtual environment as Jupyter kernel
python -m ipykernel install --user --name=venv --display-name "Python (venv)"

### Start Jupyter Notebook
jupyter notebook


### utils_scFBApy.py and pipeline_scFBApy.py files are from actual source of scFBApy.

## 3. Notebook 
Download the dataset from: https://zenodo.org/records/15072628/files/HECA-Subset.h5ad and put it in datasets folder. Run the notebook from the begining. If you don't want to run the flux generation portion you can ignore it. Because the csv file created by the flux generation code is already saved in  top_60_flux_results.csv. Above codes from flux generation can be run by using this file.