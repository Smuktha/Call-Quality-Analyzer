# Call Quality Analyzer

This project is my assignment submission for the Voice AI startup. I have implemented a Call Quality Analyzer using Python in Jupyter Notebook.

## Overview
The system analyzes a sales call transcript and outputs:
- Talk-time ratio (percentage each speaker spoke)
- Number of questions asked
- Longest monologue
- Call sentiment (positive, negative, or neutral)
- One actionable insight

## Approach
I used Jupyter Notebook to build and test this project. The input is a plain text transcript where each line is labeled with the speaker (for example: "Sales Rep:" or "Customer:"). The program parses the transcript and applies simple text processing to extract metrics.

The analysis includes:
- Counting words per speaker to calculate talk-time ratio
- Detecting questions based on question marks and common question words
- Finding the longest monologue by word count
- Performing a basic sentiment check using positive and negative keywords
- Generating an actionable insight based on who dominated the call

## Sample Output
```

{
"talk\_ratios": {"Sales Rep": 56.1, "Customer": 43.9},
"questions\_total": 2,
"questions\_by\_speaker": {"Customer": 2},
"longest\_monologue": "9 words by Sales Rep",
"sentiment": "Positive",
"insight": "Sales Rep dominated the call. Try balancing conversation."
}


---
