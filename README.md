# Data-Analysis-on-StackOverflow-Data
Data analysis on data from stackoverflow. 
## Overview
Data Science is a fast evolving field. As a data scientist, it is important for all of us to keep ourselves updated with all the new technologies, challenges and  changes happening in the data science world.
What tools are all the data scientists using today?
Are these softwares/libraries fully developed? Do they have a lot of bugs to be fixed?
Is there a strong interactive community to help with these tools?
What better way to keep track of the trends in data science than to analyze data from the largest community for developers?
Analyzing posts and interactions on Stack Overflow over a year would give us a clear idea of what is going on in the world of data science.

## The Data
The basic data file "QueryResults.csv" was extracted from data.stackexchange.com
This file contains all the posts from StackOverflow for the year 2022 which had the tag "data-science" in them.

## Project Structure
### Slides
- StackOverflow Data Analysis.pptx: Slides that explain the project
### data:
- QueryResults1.csv: Main posts data that we scraped from data.stackexchange.com. Every other data file was created through a program in the project using this.
- QueryCleaned.csv: Cleaned data created in "Data Wrangling.ipynb"
- Inverted_index.txt: Inverted index text file output from mapreduce function in "Data Wrangling.ipynb"
- WordTuple.txt: Intermediate result of MapReduce. Also a file that was created in "Data Wrangling.ipynb"
- inverted_index.csv: Made by combining Inverted_index.txt files in program "EDA.ipynb" 
- WordTuple.csv: Made by combining WordTuple.txt output files in program "SaveWordTuple.ipynb"
- cleaned_data.text: Intermediate file saved for mapreduce function in program "Data Wrangling.ipynb"

### notebooks:
- Data Wrangling.ipynb: Notebook for loading, cleaning and processing data to get it in the right format. includes the MapReduce module. Majority of data files are created here.
- EDA.ipynb: Contains basic EDA and charts that helped answer few research questions.
- SaveWordTuple.ipynb: Notebook to save the intermediate map file that was created (WordTuple.txt) into a csv file (WordTuple.csv) for use in PowerBI.
- TextAnalytics.ipynb: Notebook for Text Analytics (Sentiment Analysis, Topic Analysis and Word Vectorization).

### powerbi:
- DataVisualization.pbix: Power BI file containing the dashboard and visualizations for the project
## Correct Order of Execution
1. View "StackOverflow Data Analysis.pptx" slides
2. Get QueryResults1.csv data
3. Run "Data Wrangling.ipynb"
4. Run "EDA.ipyn"
5. Run "TextAnalytics.ipynb"
6. (optional) Run "SaveWordTuple.ipynb"
7. Open "DataVisualization.pbix" in PowerBI.
