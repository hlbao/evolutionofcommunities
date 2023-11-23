# sponsorship and co-sponsorship of House bills

Note:
1. This data set collects the long-term sponsorship and co-sponsorship behaviors on House bills among senators. It was initially built for the empirical study aligned with the modeling research on the coevolution of social communities and behaviors working with Zachary Neal and Wolfgang Banzhaf. Created by Honglin Bao, 2019 summer. We release it for open science.

2. All vote_number and vote_number_name files are data for congresses 101-110. It is separated across congresses and sessions. For example, vote_109_1 has votes from the 1st session of the 109th congress. For each bill, there are two lines in the file: the 1st line is the bill number and date, the 2nd line has 100 characters Y, N, -. File vote_109_1_names has one line per bill containing names of senators, party, and state. They are ordered according to votes in the vote_109_1 file. Sometimes it happens that senators change between the 1st session and the 2nd session, so votes in the column, say, do not always correspond to one senator. Therefore names file should be referenced.

3. Another important file is "sponsorship with time in CSV.csv." It is different from the original data file (voting normalized with 1, -1, 0 without time). In this file, I scraped congress.gov constructing a CSV file that contains (the 109th congress senator network, the 1st session (2005), and the 2nd session (2006)):

(A) A row for each legislator in this chamber;

(B) A column for each bill introduced (not just voted on) during these two sessions;

(C) Each cell contains the date that the row legislator sponsored the column bill or is blank if the row legislator did not sponsor the column bill.

