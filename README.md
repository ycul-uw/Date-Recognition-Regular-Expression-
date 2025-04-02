# Temporal Named Entity Extraction

## Problem Description

This program extracts temporal named entities (such as dates, times, and holidays) from input text using regular expressions. It identifies various date formats including full dates, months, years, and specific holidays, and outputs the results to a file.

## Recognized Date Types

The program is capable of recognizing a wide variety of temporal expressions, including but not limited to:

1. **Full Dates**:
   - "He will arrive on January 5th, 2015."
   - "May 13, 2007 was a Sunday."
   - "November 29th was on a Monday, in the 49th week of 1948."
   - "How fortunate that the world did not end on Friday, December 21st, 2012!"
   - "Today is the 1st of January, 2020."
   - "It should fall between the two calendar dates, 1/1/2020 and 2/1/2020."

2. **Partial Dates**:
   - "Sam was born in May."
   - "Her grandmother was born in 1935."
   - "June is my favorite time of the year!"

3. **Day References**:
   - "We fly to Denver on Monday."
   - "It was a Tuesday afternoon."

4. **Holidays**:
   - "We will revisit this after Labor Day."
   - "National Boyfriend Day (sometimes referred to as National Boyfriend’s Day) on October 3rd recognizes the sweetheart in your life."

5. **Special Formats**:
   - "He was born on the 13th of May."
   - "What happened then was an introduction to the events of September 11, 2001."
   - "What is celebrated every year on the 5th of May?"
   - "Do we work on May 5th?"

6. **Invalid Dates**:
   - "What happened on May 32nd?" (The program can identify and flag invalid dates.)

7. **Ambiguous Contexts**:
   - "June is my best friend." (The program distinguishes between temporal and non-temporal uses of words like "June.")

This comprehensive recognition ensures that the program can handle a wide range of temporal expressions in diverse contexts.

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
