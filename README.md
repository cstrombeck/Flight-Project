Note: This was my final project as part of the 11-week Data Science class I completed at General Assembly in New York. 
Please check back for updates (incorporating new data, using alternative models and adding more visualizations) in early 2016. 

# Does the Existence of Baggage Fees Delay Flights?


## Aim & Hypothesis  

The aim of this project was to determine whether there is a statistically significant difference in actual flight time performance between airlines with versus without baggage fees.  
The hypothesis is that airlines that charge a fee for checking baggage will have longer flight times. The reasoning being that when airlines charge passengers for checking bags, passengers are more likely to bring their luggage on board as a carry-on, which leads to added difficulties in finding space in the overhead compartments, prolonging boarding times and delaying flights.   This would be an additional factor against traveling on airlines that charge a baggage fee, which could be valuable for passengers to consider in their choice of airlines. 

_See_ `Final Project Presentation.pptx` _for project overview and findings._


## Code  

The python code is organized in sections and well documented in the iPython notebook: `Final Project.ipynb`

* **Data Exploration and Processing:** The data is reviewed for availability and correctness of information.   
Additional variables are added, time measurements are calculated, airline information is updated and the data is limited to the 20 most common routes. 
* **Modeling:** The actual statistical analysis is implemented using multiple linear regression with dummy variables for the origin airport, the destination airport, the airline and the existence of bag fees. Various sensitivities are carried out. 

_See_ `Final Project Paper.docx` _for more detailed information._


## Data   

       Type         |                  Filename(s)            |                 Source                    |  Link to Data  |                         Dictionary
--------------------| ----------------------------------------| ----------------------------------------- | ---------------| --------------------------------------------------------------------------  
   Flight Data      |`On\_Time\_On\_Time\_` <br> `Performance\_*year\_month*`| Bureau of Transportation Statistics (BTS) | [BTS Data] (http://www.transtats.bts.gov/DL\_SelectFields.asp?Table\_ID=236) | [BTS Data Dictionary] (http://www.transtats.bts.gov/DL\_SelectFields.asp?Table\_ID=236) <br> [BTS Data Glossary](http://www.transtats.bts.gov/glossary.asp) <br> `Flight Data_readme.html`
   Airline Names    |             `L\_AIRLINE\_ID.csv`        | Bureau of Transportation Statistics (BTS) | [BTS AirlineID Lookup Table] (http://www.transtats.bts.gov/DL\_SelectFields.asp?Table\_ID=236) | 
 Airport Coordinates|  		   	 `global\_airports.csv`       |           openflights.org                 | [Datahub page] (https://datahub.io/dataset/global-airports) | [Datahub page] (https://datahub.io/dataset/global-airports)
   Baggage Fees     |           `AIRLINE\_FEES\_man.csv`      |     Manually collected from sources       | [Tripadvisor] (http://www.tripadvisor.com/AirlineFees) <br> [AirfareWatchDog] (http://www.airfarewatchdog.com/blog/3801089/airline-baggage-fees-chart/) <br> [Seatguru] (http://www.seatguru.com/airlines/Spirit_Airlines/baggage.php) <br> + Airline-specific sites 
   
The Flight Data has not been included in this repository, but can be downloaded via the link to BTS above. 