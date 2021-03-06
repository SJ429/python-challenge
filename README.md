
## Welcome to the World of Programming with Python.


It's time to put away the Excel sheet and join the big leagues. 

Python scripts were created to analyze the financial statements of PyBank and the election result of PyPoll.

## Process

Therefore, the os module was imported to create file paths across operating systems.

Additionally, module for reading CSV files was imported.

To run code, set the path for file, open and read CSV 

with open(csvpath) as csvfile. 

 CSV reader specifies delimiter and variable that holds contents with: 
 
     csvreader = csv.reader(csvfile, delimiter=',')
     
     print(csvreader)

 Read the header row first 
    csv_header = next(csvreader)
   
 Read each row of data after the header
    for row in csvreader:
    
Then iterate through each line to perform calculations and write the results to a new csv file.

## PyBank
PyBank’s dataset is composed of two columns: `Date` and `Profit/Losses`.  

The scripts calculated the following:
  
    * The total number of months included in the dataset
    
    * The net total amount of "Profit/Losses" over the entire period
    
    * The average of the changes in "Profit/Losses" over the entire period
    
    * The greatest increase in profits (date and amount) over the entire period
    
    * The greatest decrease in losses (date and amount) over the entire period

  Financial Analysis
  ----------------------------
  Total Months: 86
  
  Total: $38382578
  
  Average Change: $-2315.12
  
  Greatest Increase in Profits: Feb-2012 ($1926159)
  
  Greatest Decrease in Profits: Sep-2013 ($-2196167)
  
  
  -------------------------

## PyPoll

PyPoll’s dataset is composed of three columns: `Voter ID`, `County`, and `Candidate`.  

The scripts calculated the following:


     * The total number of votes cast
     
     * A complete list of candidates who received votes
     
     * The percentage of votes each candidate won
     
     * The total number of votes each candidate won
     
     * The winner of the election based on popular vote.

  Election Results
  -------------------------
    Total Votes: 3521001
  -------------------------
  
   Khan: 63.000% (2218231)
   
   Correy: 20.000% (704200)
   
   Li: 14.000% (492940)
   
   O'Tooley: 3.000% (105630)
      
   -------------------------
   Winner: Khan
  -------------------------
