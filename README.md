# Goodreads - Quotes - User Interface
This is an User Interface to get the top 10 quotes by Mark Twain from goodreads.com through a script running behind the scenes once the application starts. My main objective while solving this exercise was to focus on the correct display of data rather than fancy way to show it.  

The script [forms.py](https://github.com/sushantgupta1206/GUPSUS03part2/blob/master/GoodReadsScrapperUI/forms.py) is the main python script to be run from a command line and it will start a server on the local host where the user is expected to enter his/ her credentials in order to view the most famous quotes by Mark Twain. The script when executed, authenticates the user to `http://www.Goodreads.com website`. The code then finds, retrieves and rebders the [html page](https://github.com/sushantgupta1206/GUPSUS03part2/blob/master/GoodReadsScrapperUI/templates/good_reads.html) on the localhost which displays the top 10 popular quotes from **Mark Twain** on the UI.      
  
  
**Technology Stack used :**   
> Python 2.7  
> Robobrowser Library in python  
> Beautifulsoup Library   
> Flask for UI creation
> wtform in python for verification  

**The Output and inferences :**   
  
Please check the output files in the output folder [here](https://github.com/sushantgupta1206/GUPSUS03part2/tree/master/Output) and the top 10 quotes the code generated [here] (https://github.com/sushantgupta1206/GUPSUS02/blob/master/Top10_Quotes.txt) to verify the correctness. Also, invalid credentials will not be authorized to see the quotes and an error/ alert is shown for the same.  
  
**Steps to Run the code:**   
> 1. clone the repository using `git clone https://github.com/sushantgupta1206/GUPSUS03part2.git` on the local machine  
> 2. Navigate to the folder `cd \GUPSUS03part2\GoodReadsScrapperUI>`  
> 3. install dependencies using `pip install bs4` for beautiful soup; `pip install robobrowser` for installing Robobrowser; `pip install flask` for the flask setup/ configuration; and `pip install wtforms` for the form validation library.  
> 4. Run the script `forms.py` by using `python forms.py`.
> 5. On the chrome/ IE browser please go the local host and port which the console specifies where the server starts: in my case it is 'http://127.0.0.1:5000/'
> 6. Enter valid user credentials and you should see the output or else it will throw invalid credential error.  

**References and Readings**
> 1. https://www.crummy.com/software/BeautifulSoup/bs4/doc/
> 2. https://robobrowser.readthedocs.io/en/latest/readme.html

**Note:**  
> The code takes time to display the results as the it reads, filters and parses data only after the button is clicked
> as a future improvement the UI can be made more decorative but currently it satisfies the requirement of clear readibility.




