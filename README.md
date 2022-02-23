# Project4
Log Parsing in Python

(Part 1 Instructions):
For this project, you will be working as a team, but will be graded individually. So each team member will be responsible to turn in a separate solution, or the whole team can collaborate in a single GitHub repo, and I will expect to see a log of individual contributions (commits from each team member).

The goal of this project is to familiarize yourself with Python syntax, and some basic tasks that are common in systems programming and administration. The program will be invoked from the command line on a fresh Linux machine, so if you introduce any library dependencies beyond the Python Standard Library (not recommended), you must provide very clear instructions to recreate your environment. I would suggest using Vagrant (Links to an external site.) or a GCP (Links to an external site.) VM to develop in Linux if you are on a Windows machine. Another option is to install the Windows Subsystem for Linux (Links to an external site.) and setup a Python environment (Links to an external site.). It is your responsibility to ensure the program runs as expected in the operational environment described.

Here’s the scenario: you work for a medium sized company that sells widgets directly to consumers through brick-and-mortar retail stores. The marketing department wants to try a new promotional campaign to ramp up direct internet sales, but needs better data about current traffic to your website. Your boss has asked you to take the HTTP server logs from the webserver and provide some analytics to Marketing.

STEPS:
1. Your program will be parsing and analyzing log files from an Apache web server. The first thing your program must do is retrieve the log file across the network. It is available here: https://s3.amazonaws.com/tcmg476/http_access_log (Links to an external site.)

2. Once you download the file, you need to save a local copy to disk (a cached copy) so the next time you run your script, you don't have to wait for the download.

3. Marketing wants to know two things: 
  How many total requests have been made in the 6 months?
  How many total requests were made in the time period represented by the log?

4. You will need to output this data to the screen. The format you choose to do this is up to you, but your decisions and your implementation should be logical and consistent.

Your program should be created and developed using GitHub (I will be examining the commit logs to see your work). When the project is due, submit your repository URL so I can clone the repo and test your program.

*********************************************************************************************************************************************************************************

(Part 2 Instructions):
Marketing was very happy with the data you provided them. Now they want more. They have asked that you answer more questions  so they have a better idea about the nature of the visitors that are coming to the company website.

Marketing is asking for answer to the following questions:

1. How many requests were made on each day? 
2. How many requests were made on a week-by-week basis? Per month?
3. What percentage of the requests were not successful (any 4xx status code)?
4. What percentage of the requests were redirected elsewhere (any 3xx codes)?
5. What was the most-requested file?
6. What was the least-requested file?

Finally, it was decided that the logs should be broken into separate files by month, so that staff in the marketing department can do further analysis. Your program should split the log file into 12 smaller files, where the data stored in each file are the log events for a single month. These should be written to disk in the same directory as your program file, in a logical and consistent manner.

Your program should be created and developed using GitHub (I will be examining the commit logs to see your work). When the project is due, submit your repository URL so I can clone the repo and test your program.  

If you are working in a pair group, each student should submit the same repo URL.
