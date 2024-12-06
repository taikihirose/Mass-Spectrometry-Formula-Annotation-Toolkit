# Mass-Spectrometry-Formula-Annotation-Toolkit
###Overview
This project is a toolkit for analyzing mass spectrometry (MS) data to generate and evaluate candidate molecular formulas. It integrates the following three tools:
1. **MS-FINDER**
2. **SIRIUS**
3. **MSBUDDY**
4. Additionally, it merges results from these tools, calculates scores, and outputs the consolidated results.

##Project Structure
The project consists of the following Python scripts:

main.py
The main entry point of the project. It automates data preprocessing, tool execution, and result integration​
.

buddy_cmd.py
Processes MGF-formatted input data with MSBuddy to annotate molecular formulas​
.

creat_summary.py
Combines output from MSFinder, SIRIUS, and MSBuddy to generate a summary file​
.

mgf_parser.py
Converts MSP files to MGF format and splits data by adduct type​
.

ms_parser.py
Reads MSP files and converts them to MS format​
.

msfinder_cmd.py
Executes MS-Finder via the command line and retrieves results​
.

scoring.py
Calculates scores for integrated results and determines the best candidate molecular formulas​
.

sirius_cmd.py
Runs SIRIUS to generate molecular formula candidates and infer structural candidates​
.

split_msp.py
Splits MSP files into separate files, one for each compound​
.

