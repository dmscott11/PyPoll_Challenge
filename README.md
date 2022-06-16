# PyPoll_Challenge
## Overview of Election Audit
The audit of election results was performed as requested by Seth and Tom. The initial candidate results were submitted to the election commission. The election commission followed up with a request to look at the individuals counties election data which includes voter turnout for each county and which county had the largest voter turnout overall. The data that was used to perform the county audit was the same data used to perform the candidate audit. 
## Election-Audit Results
As seen in the image below, the results of running the election data throught the created python code are as follows:

![](/images/Terminal_Output.png)

To make it more clear: 
* Denver made up both the largest total voter turnout with 306,055 total votes and 82.8% of total voter turnout.
* Jefferson County was second with 38,855 total votes and 10.5% of total voter turnout.
* Arapahoe County was last third with 24,801 total votes and 6.7% of total voter turnout. 

These counties combined gave us 369,711 total votes which matches the total votes determined in the initial candidate analysis. 

## Election-Audit Summary
In summation, this python code can be reapplied in future years to perform audits on election data by both candidate and county identifiers. The code may require refactoring depending on the format desired for the output and the format of the data initially. As an example two changes to the python code provided could be:
- A change that might need to be made based on the .csv file being read are on lines 50 and 53. These could potentially need to have their index altered if the format of the .csv file is different. 
  
  -``county_name = row [1]``
  
  -``candidate_name = row[2]`` 

- Another change that might need to be made when reusing the python code included would be on lines 10 and 12. These would change depending on the file structure of the person running the code and the file names for the .csv file being read and the .txt file being written to. 

  -`file_to_load = os.path.join("Resources", "election_results.csv")`
  
  -`file_to_save = os.path.join("analysis", "election_analysis.txt")`
