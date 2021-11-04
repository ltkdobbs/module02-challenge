# **Analysis – Stock Comparison 2017-2018**
## **Background Breakdown**
The Client’s (Steve) major focus was on diversifying his client’s stock portfolio; the information provided suggest that a majority of their portfolio involved investments was in the company DAQO New Energy Corp (Stock Ticker DQ). Through VBA coding, our goal was to build a macro which would allow the Client to run an analysis on a list of stock within the document with the press of a button.
Currently, the Client is limiting themselves to twelve stock options, and the data only covers two years. A solid starting point, but the ideal end goal is a macro which works if and when the Client decides to branch out to more stocks, or a larger range of years.
## **Challenges**
The biggest challenge I can foresee is when the Client inevitably wants to analyze a wider range of stocks. While not an overly difficult adjustment, if the number of stocks is unknown, it would require a workaround which is currently beyond our current skill level. Not impossible, but far more time consuming to do.
## **Results**
### Stock Performance between 2017 and 2018
From what we can see in the tables generated (See Image 1.1, All Stocks 2017, and Image 1.2, All Stocks 2018 below), 2017 was overall a better year for the stocks the Client chose to investigate. Only one stock, TERP, had a negative yearly return (-7.2%), while the other eleven stock options had positive returns; several even surpassed a 100% return. Unfortunately, many of those stocks didn’t fare as well in 2018.
Out of the twelve stocks listed, ten had negative returns; of those, two had negative returns over fifty percent – one of which was the major component in the portfolio the Client is reviewing (Stock Ticker DQ, with a return of -62.6%). The two stocks which did well in 2018 were ENPH and RUN, with an 81.9% and 84.0% return respectively.

###### Image 1.1 All Stocks 2017 & Image 1.2 All Stocks 2018

![All Stocks 2017](https://github.com/ltkdobbs/module02-challenge/blob/main/All_Stocks_2017.png)
![All Stocks 2018](https://github.com/ltkdobbs/module02-challenge/blob/main/All_Stocks_2018.png)
#### Refactoring
In terms of refactoring, the difference in run speed is impressive; the refactored code is roughly 89.68% faster for the 2017 analysis and 88.48% faster for the 2018 analysis, taking less than one twentieth of a second to process either data set.
By comparing Image 1.3 and 1.4, we can see the run time in seconds for pre-refactored and post-refactored runs of the 2017 data set below (see Images 1.3 and 1.4). The final run time pre-refactoring is 1.628906 seconds, which isn’t very long really. But in comparison, the refactored code runs in 0.1679688 seconds – less than half a second, while the original code took nearly two! We see a similar result in the analysis for 2018; the pre-refactoring run time is 1.59375 seconds, versus the 0.1835938 seconds runtime post-refactoring (see Images 1.5 and 1.6)!

###### Image 1.3 Module 02 Macro Time 2017 & Image 1.4 Refactored Macro Time 2017

![2017 Module Time]( https://github.com/ltkdobbs/module02-challenge/blob/main/Module_02_2017.png)
![2017 Refactored Time]( https://github.com/ltkdobbs/module02-challenge/blob/main/Challenge_Macro_2017.png)

###### Image 1.5 Module 02 Macro Time 2018 & Image 1.6 Refactored Macro Time 2018

![2018 Module Time]( https://github.com/ltkdobbs/module02-challenge/blob/main/Module_02_2018.png)
![2018 Refactored Time]( https://github.com/ltkdobbs/module02-challenge/blob/main/Challenge_Macro_2018.png)

## **Limitations**
1)	The biggest limitation right now, is that the macro is coded to handle a total of 12 tickers. If the Client is interested in analyzing more, then the code will have to be edited to accommodate.
2)	The current data sets don’t offer any concrete long-term trends for any of the stocks investigated. While easily rectified, it does give a skewed view of the data, and should be considered.
## **Summary**
### Advantages of Refactoring
As a general rule, refactoring optimizes and condenses code into a more palatable and effective configuration. Ideally, it reduces clunky workarounds and patch jobs, usually by reevaluating code and finding more effective methods to achieve the same goal. Rearranging, exchanging, cutting, and general tweaking builds a better, more reliable code – a lofty but often achievable goal.
By refining the code, specifically by introducing more flexible variables and multiple arrays, we also streamlined the functionality, not just in run-time (see Results) but also in reducing the among of tinkering necessary for alterations. Currently, the script runs for the twelve stock tickers the Client is investigating.
In the previous code, though it wouldn’t be difficult to increase the number of stock tickers, the methodology of the instructions would slow down the run time even more, causing the analysis to take far more time; as it stands, the refactored code has the computer clear the Volume values during each loop, leaving less room for error, while also formatting the table – something left to a separate script in the prior incarnation.
### Disadvantages of Refactoring
The disadvantage is that one can easily be bogged down with the knowledge of what does work, and refining takes time. Part of refactoring means pushing aside code which, ostensibly, works, in order to make it better. Pulling pieces and adjusting syntax is time consuming, and it can become both mind numbing and overwhelmingly frustrating to review the same section of code again and again in order to refine everything just right.
Refactoring also means rewriting in many cases – which can be an annoyance when the code does what it needs to do. Overall, the process is no different from writing the code in the first place; it still requires extensive debugging, persistent review, and double-checking syntax, variables, arrays, and all the other pieces to make sure every cog and gear is in place.
