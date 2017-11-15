# Twitter-Sentiment-Analysis

This folder consists of the python code “twitter_sentiments.py” and the data collected so far.

How to run the python code?

The purpose of this python file is to find tweets based on the certain query and then write them into a csv file with some of the tweet’s attributes.

In order to run this file, you first need to create a file called “auth.k”

Open emacs/vim for a file “auth.k”
Based on your twitter organization account, select those 4 lines and then copy paste them into this file.
Ordering does matter, so put them in the same order
Save the file.

To change the keyword:
Navigate to line 29 in the python code.
Change the query to whatever you want it to be
Run the file using Anaconda Prompt

How the results are saved:
The results are saved in a csv file in the format,
Results- +
Query name (Keyword used) +
Current day (which day you ran the code) +
Current time (What time you ran the code)

What needs to be done next?

There are a lot of csv files with different keywords used.
I need you to start grouping them together based on keyword
Separate all the files based on keyword
Concatenate them
I think the count goes wrong if you don’t remove the blank spaces between the files.
So, please remove the blank spaces in each file.
And then concatenate them using the code I’ve given below

Import pandas as pd

stressData1 = pd.read_csv('results_stress.csv')
stressData2 = pd.read_csv('resultStress2.csv')
frames = [stressData1, stressData2]
fullStress = pd.concat(frames)
fullStress.to_csv('fullStress.csv', sep = ',')

You can do this for multiple frames.
For example using the keyword “stress”

Have stress1, stress2, …
Concatenate all them together
And then save it into a final csv file for the keyword

Message me if you have any questions.


