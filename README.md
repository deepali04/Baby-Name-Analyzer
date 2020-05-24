## Introduction

 The project determines the popularity of different baby names in the US over time by analyzing input data files. It is a part of an undertaken java course in which most of the work done on the concepts of **Java Strings** and **Java File Handling**.

## Information about Data

The data here contain the baby names from the United States year wise. The input files are .csv files for each year in format **"yob20XX.csv"**.
The file contains name, gender, number of babies having that name in that particular year.

for eg: Emma,F,20566 (1 row in a file yob2014.csv )

## Functionalities

There are various functions we are writing to analyze the file.

* **totalBirths (FileResource fr):** The function takes file as an argument and retrives total number of unique girls names, the number of unique boys names and the total names in the file.

* **getRank (int year, String name, String gender):** The function takes three parameters year, name and gender (F for female and M for male). It returns the rank of the name in the file for the given gender.
Rank 1 is the name with the highest number of births. If the name is not in the file, then -1 is returned. 
