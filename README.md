## Introduction

 The project determines the popularity of different baby names in the US over time by analyzing input data files. It is a part of an undertaken java course in which most of the work done on the concepts of **Java Strings** and **Java File Handling**.

## Information about Data

The data here contain the baby names from the United States year wise. The input files are .csv files for each year in format **"yob20XX.csv"**.
The file contains name, gender, number of babies having that name in that particular year.

for eg: Emma,F,20566 (1 row in a file yob2014.csv )

## Functionalities

There are various functions to analyze the file of baby names.

* **totalBirths (FileResource fr):** The function takes file as an argument and retrives total number of unique girls names, the number of unique boys names and the total names in the file.

* **getRank (int year, String name, String gender):** The function takes three parameters year, name and gender (F for female and M for male). It returns the rank of the name in the file for the given gender.
Rank 1 is the name with the highest number of births. If the name is not in the file, then **-1** is returned.

* **getName (int year, int rank, String gender):**  The function takes three parameters year, rank and gender (F for female and M for male). It returns the name of the person in the file at this rank.
Rank 1 is the name with the highest number of births. If the rank does not exist in the file, then **“NO NAME”** is returned.

* **whatIsNameInYear (String name, int year, int newYear, String gender):** The method has four parameters: a string name , an integer  year representing the year that name was born, an integer newYear and a stringnamed gender (F for female and M for male). It determines what name would have been named if they were born in a different year, based on the same popularity. It determines the rank of name in the year they were born, and then print the name born in newYear that is at the same rank and same gender.
Eg: Isabella born in 2012 would be Sophia if she was born in 2014.

* **yearOfHighestRank (String name, String gender):** The method takes two parameters, a string name and a string gender (F for female and M for male). It selects a range of files to process and returns an integer, the year with the highest rank for the name and gender. If the name and gender are not in any of the selected files, it will return **1**.

* **getAverageRank (String name, String gender):** This method takes two parameters, a string name and a string gender (F for female and M for male). It selects a range of files to process and returns a double representing the average rank of the name and gender over
the selected files. It should return **1.0** if the name is not ranked in any of the selected files.

* **getTotalBirthsRankedHigher (int year, String name, String gender):** This method takes three parameters, an integer year, a string  name and a string gender (F for female and M for male). It returns an integer, the total number of births of those names with the
same gender and same year who are ranked higher than name.

* **printNames():** This methos prints data from file like how many babies are having any particular name. For eg: Emma,F,20456 (There are 20456 female babies having name Emma).

## Compiling and Running the file

* **For Compilation:** Java RankNames.java

* **For Running:** java RankNames

Here RankNames in filename

