# evolution of social communities: an agent-based approach
Notice some tips:
1. All vote_number and vote_number_name files are data for congresses 101-110. It is separated across congresses and sessions. For example, vote_109_1 is has votes from 1st session of the 109th congress. For each bill, there are two lines in the file: 1st line is the bill number and date, 2nd line has 100 characters Y, N, -. File vote_109_1_names has one line per bill, containing names of senators, party and state. They are ordered according to votes in the vote_109_1 file. Sometimes it happens that senators change between 1st session and 2nd session, so votes in column, say, 23 do not always correspond to one senator. Therefore names file should be referenced.

Another important file is "sponsorship with time in CSV.csv". It is diffferent with the original data file (voting nornalized with 1, -1, 0 without time). In this file, I scraped congress.gov constructing a CSV file that contains (notice also 109th congress senator network, the 1st session (2005) and the 2nd session (2006)):
(A) A row for each legislator in this chamber
(B) A column for each bill introduced (not just voted on) during the these two sessions
(C) Each cell should contain the date that the row legislator sponsored the column bill, or should be blank if the row legislator did not sponsor the column bill.
