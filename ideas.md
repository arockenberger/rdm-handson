# Collection of ideas

## Scope

- develop short hands-on workshop based on the article "Good Enough Practices in Scientific Computing" by Wilson et al. 2017
- workshop could be conceptualized as a supplementary hands-on part to the research data management workshops at UiO
- could serve generally as guide to good practice (if instructions are brief and executable)


## Excerpts from the article

### Introduction

*ALWAYS add page numbers for both paraphrases and direct quotes from the article!*
- target audience of article - and of workshop - is researchers from any field who are novices in programming and data wrangling: people who are using a computer mostly every day for work, study, leisure, but who do not do any programming and mainly use proprietary office software, applications that run in a browser and perhaps domain specific software and applications
- additionally: researchers who work alone or with a few collaborators on projects lasting a few days to several months (this is very often the case for graduate students; it is also widely the modes operandi in the Humanities)
- goal: which are the first accessible skills and perspectives any such learner needs to develop? (p.2)
- "minimum set of tools and techniques […] every researcher can and should consider adopting" (p.2)

**Main Topics**

1. Data management
2. Code (Software / Programming)
3. Collaboration
4. Project Organisation
5. Tracking changes
6. Writing manuscripts

- could be used to structure the workshop into units / episodes

### Data Management

#### STEP 1
- make copy of raw data
- enable read-only access to raw data file
- alternatively: record exact procedure used to obtain raw data + other pertinent info (version nr., date of download etc.)

#### STEP 2
- ensure reliable back-up is in place (check with local IT)
- make use of cloud services (check with your institutions regulations and check if your data requires certain security routines)
  - check with the traffic-light codes for Data
  - GREEN data should be fine with almost all services

#### STEP 3
- create usable data, in open formats (think .csv instead of .xlsx for tables; think .xml, .json, .yaml for non-tabular data (trees, graphs), etc.)
  - find some good examples from different fields of research here!
- usable means for both humans and machines
- variable names should be human-readable ("tidy data")
- clear, human and machine readable filenames without whitespace

#### STEP 4
- create analysis-friendly data
  - each column is a variable
  - each row is an observation

#### STEP 5
- record all steps used to process data
  - preferably, every time changes are made to the data, a script is written an preserved
  - e.g. using ```pandas``` (Python package) to rename columns, step-by-step [here](https://cmdlinetips.com/2018/03/how-to-change-column-names-and-row-indexes-in-pandas/)
  - alternatively, you could document each step of manual data manipulation
  - how about using OpenRefine? Can the scripts be exported for documentation?

#### STEP 6
- use unique keys or IDs to link Data

#### STEP 7
- publish your data
- assign it a DOI (if possible)
- share!
- metadata and README
- write modular code, i.e.
  - create functions (readable, reusable, testable)
  - give functions and variables meaningful names

#### STEP 8
- publish your code and assign it a DOI
  - example: use Zenodo with GitHub
- code is research too!

**The overall goal is to have data that is clean and tidy**

### Code (Software)

- who? a researcher writing a few dozen lines of code now and again, probably for themselves
  - what about re-using someone else's code or parts of it?  
