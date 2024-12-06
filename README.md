# Mass Spectrometry Formula Annotation Toolkit

## Overview
This project is a toolkit for analyzing mass spectrometry (MS) data to generate and evaluate candidate molecular formulas. It integrates the following three tools:

1. **MS-Finder**  
2. **SIRIUS**  
3. **MSBuddy**

Additionally, it merges results from these tools, calculates scores, and outputs the consolidated results.

---

## Project Structure

The project consists of the following Python scripts:

- **`main.py`**  
  The main entry point of the project. Automates data preprocessing, tool execution, and result integration.

- **`buddy_cmd.py`**  
  Processes MGF-formatted input data with MSBuddy to annotate molecular formulas.

- **`creat_summary.py`**  
  Combines output from MSFinder, SIRIUS, and MSBuddy to generate a summary file.

- **`mgf_parser.py`**  
  Converts MSP files to MGF format and splits data by adduct type.

- **`ms_parser.py`**  
  Reads MSP files and converts them to MS format.

- **`msfinder_cmd.py`**  
  Executes MS-Finder via the command line and retrieves results.

- **`scoring.py`**  
  Calculates scores for integrated results and determines the best candidate molecular formulas.

- **`sirius_cmd.py`**  
  Runs SIRIUS to generate molecular formula candidates and infer structural candidates.

- **`split_msp.py`**  
  Splits MSP files into separate files, one for each compound.

---

## Installation

1. Clone this repository:
   ```bash
   https://github.com/taikihirose/Mass-Spectrometry-Formula-Annotation-Toolkit/blob/main/README.md

2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt

3. Download and install the necessary tools (SIRIUS, MS-Finder) from their official websites.

---

## Usage
1. **Run the project:**
   ```bash
   python main.py

You will be prompted to provide the input file path and SIRIUS login credentials during execution.

2. **Output Result**
・ Consolidated results will be saved as a CSV file in the summary_output directory.
・ Scored results will be output as rescoring_formula.csv.

---

## Requirements
**・ Python 3.12+**
**・ External tools**
・ MS-FINDER
・ SIRIUS
・ MSBUDDY

# Project Folder Structure

## Required Files and Directories

To properly set up and run the project, ensure the following files and directories are present and correctly placed:

### 1. Directories
- **`msfinder/`**  
  This directory should contain the MS-FINDER software version 3.60. Place the software's executable and related files inside this folder.  

  **Download from Google Drive**: [Google Drive](https://drive.google.com/drive/folders/0AIZ5vTceA0LvUk9PVA)

- **`sirius4/`**  
  This directory should contain the SIRIUS version 4 software. Include the `sirius.exe` file and all necessary subfolders provided by the software installation.  

  **Download from Google Drive**: [Google Drive](https://drive.google.com/drive/folders/0AIZ5vTceA0LvUk9PVA)

---

## Folder Structure Example

Below is an example of how the project directory should look:


