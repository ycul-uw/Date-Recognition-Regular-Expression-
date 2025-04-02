# Temporal Named Entity Extraction

## Problem Description

This program extracts temporal named entities (such as dates, times, and holidays) from input text using regular expressions. It identifies various date formats including full dates, months, years, and specific holidays, and outputs the results to a file.

## How to Run the Code

1. **Input File**: Place your input text file in the `../Data/Input/` directory. The file should contain text from which you want to extract temporal entities.
2. **Run the Program**: Execute the Python script:

   ```bash
   python extract_temporal_entities.py
   ```

3. **Output**: The program will process each line of the input file and save the extracted temporal entities in the `../Data/Output/output.txt` file.

### Requirements

- Python 3.x
- No external libraries are required, as the program only uses built-in Python functionality (e.g., `re` for regular expressions).
