This project is based on "The Complete Pandas Bootcamp 2023 - Data Science with Python," a course offered by Udemy and taught by Alexander Hagmann. It presents a Data Aggregation challenge, requiring the application and combination of various concepts and methods.

This challenge is commonly used in job application processes and assessment centers within the field of Data Science. It tests candidates' abilities to work with, manipulate, and aggregate data. Even experienced Data Scientists find it challenging, not due to its coding complexity, but because it demands:

- Proficient coding skills, and more importantly,
- The capability to interpret and understand the underlying data, incorporating insights from subject matter experts—in this case, sports experts.

Emphasis is placed on "Thinking in Data Structures!"

**Project Goal:**
On your first day at a Data Science advisory firm, your task is to produce the official Summer Olympic Games Medal Tables for all editions from 1896 to 2012.

You are provided with a dataset containing over 31,000 medals (summer.csv) and the official Medal Tables for the 1996 and 1976 editions from Wikipedia (wik_1996.csv, wik_1976.csv). These official Medal Tables serve as a reference to verify the accuracy of your code.

Your objective is to minimize the divergence between your aggregated Medal Tables and the official Medal Tables. For example, if the official count of Gold Medals for the United States in the 1996 edition is 44, and your code calculates 46, this represents an absolute divergence of 2.

Calculate the total absolute divergence for the 1996 and 1976 editions (the "Score"). The optimal Score is 0!

**Valuable Insights from Sports Experts:**
- In Team Events, each medal awarded to individual team members counts as a single medal. For instance, the United States Basketball Team winning a Gold Medal in 2012, with 12 athletes, counts as one Gold Medal in the official 2012 Medal Table.
- Events with 5 or fewer medals are considered Singles Events, and those with more than 5 medals are Team Events. In Singles Events, all awarded medals (including shared Bronze medals, leading to 4 or 5 medals in total) count for the official Medal Table. The same applies to Team Events where two teams may share the Bronze medal, resulting in a total of 4 medals (1 Gold, 1 Silver, 2 Bronze) for the Medal Table.
- To identify unique events, the gender category of the event is crucial. There are Men's, Women's, and Mixed Events. Mixed Events can be identified as those marked "mixed" or "pairs," all "Equestrian" events, "Sailing" events before 1988, and certain specified medals in Badminton mixed doubles.

Embark on this challenge and showcase your data science skills!

To identify all unique Events, the Event Gender matters! There are Men Events, Women Events and Mixed Events. Assume
that the following medals have been awarded in Mixed Events:

- the Event is marked with "mixed" or "pairs"
- all "Equestrian" Events
- all "Sailing" Events before 1988 (until and including 1984)
- the following medals (index labels) were awarded in Badminton mixed Double Events: [21773, 21782, 21776, 21785, 21770,
21779, 23703, 23712, 23706, 23715, 23709, 23700, 25720, 25729, 25723, 25732, 25726, 25717, 27727, 27736, 27730, 27739,
27724, 27733, 29784, 29785, 29786, 29787, 29788, 29789]