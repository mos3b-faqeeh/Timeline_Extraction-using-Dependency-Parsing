# Event Timeline Extraction from Text using Named Entity Recognition and Dependency Parsing

This repository contains a notebook that demonstrates how to extract a timeline of events from a text document using Named Entity Recognition (NER) and dependency parsing techniques. The goal is to automatically generate a timeline similar to the one found in the [Wikipedia article on the History of Germany](https://en.wikipedia.org/wiki/History_of_Germany).

## Overview

The notebook provides a step-by-step guide to extract events and their corresponding dates from a given text. The extracted events are then compiled into a timeline format, where each event is associated with a specific date.

### Example

Given the text:

> On March 1st 2020, Joe Biden wins the South Carolina primary.

The notebook extracts the event:

> [2020/03/01] - [Joe Biden wins the South Carolina primary]

Similarly, the notebook processes larger documents, such as a Wikipedia article, to generate timelines like:

| Date    | Event                                                                                         |
|---------|-----------------------------------------------------------------------------------------------|
| 1338    | The prince-electors of the Holy Roman Empire declared in the Declaration of Rhense...         |
| 1356    | The Imperial Diet issued the Golden Bull of 1356...                                           |
| 1370    | The Treaty of Stralsund was signed...                                                         |
| 1400    | The period of Meistersinger lyric poets began.                                                |

## Methods Used

- **Regular Expressions**: Initially, simple regex patterns are employed to capture dates and events.
- **spaCy**: The core of the extraction relies on spaCy's Named Entity Recognition (NER) and dependency parsing features to identify and extract events associated with specific dates.

## Installation

To run the notebook locally, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/event-timeline-extraction.git
   cd event-timeline-extraction


Usage
The notebook event_timeline_extraction.ipynb demonstrates how to:

Load and preprocess text.
Extract events using regex.
Enhance extraction using spaCy's NER and dependency parsing.
Generate and display a timeline of events.
Feel free to modify the notebook to process different documents or adjust the extraction methods to suit your needs.

Contributions
Contributions are welcome! If you find any issues or want to add features, please feel free to open a pull request or raise an issue.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgements
The spaCy library for providing robust NER and dependency parsing functionalities.
Wikipedia for providing comprehensive articles that serve as a testbed for this project.
