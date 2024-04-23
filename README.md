# LA Times Search Engine
This is a Search Engine for LA Times articles built-in Python. This program was created during the course "MSCI 541 Search Engines" for our term-long project.
The corpus is LA Times articles from gathered from 1989-1990. This is a TREC dataset.

## Installation Requirements:
1.	Please install Python on your computer before running the program.
2.	Clone the repository on your device by entering this into your terminal: git clone https://github.com/matterxleben/Search-Engine.git

## Running the Programs:
To run these programs, please navigate to where you cloned the repository and open the working directory .../msci-541-f23-hw5-matterxleben


### IndexEngine: 
This program accepts two command line arguments:
1.	a path to the latimes.gz file
2.	a path to a directory where the documents, metadata, and term files will be stored.

For example, you would run IndexEngine from the command prompt / terminal / shell as:
python IndexEngine.py C:/Users/matth/OneDrive/Desktop/University/3B/MSCI541-Search-Engines/HW5/raw-data/latimes.gz C:/Users/matth/OneDrive/Desktop/University/3B/MSCI541-Search-Engines/HW5/store

### BM25SearchEngine: 
The program does not expect command line arguments to run. The program can be run by simply running the program (through and IDE or through the terminal). The program will prompt a user input through the terminal command prompt / terminal / shell, which will be the first query for the user to enter. 
For this program, the location of the inverted index and other term files folder is in the code for the program, the path is hardcoded as:
term_files_path = "C:/Users/matth/OneDrive/Desktop/University/3B/MSCI541-Search-Engines/HW5/store/term_files"
store_path = "C:/Users/matth/OneDrive/Desktop/University/3B/MSCI541-Search-Engines/HW5/store"
Please change this to your own computers path folder to obtain term files!

### ResultsEvaluation:

The program accepts 2 command line arguments: 
1. the directory location of your results file
2. the directory location of your qrels file

For example, you would run ResultsEvaluation.py from the command prompt / terminal / shell as:
    python ResultsEvaluation.py C:/Users/matth/OneDrive/Desktop/University/3B/MSCI541-Search-Engines/HW4/msci-541-f23-hw4-matterxleben/results/hw4-bm25-baseline-merxlebe.txt C:/Users/matth/OneDrive/Desktop/University/3B/MSCI541-Search-Engines/HW4/hw3-files-2023/qrels/LA-only.trec8-401.450.minus416-423-437-444-447.txt
