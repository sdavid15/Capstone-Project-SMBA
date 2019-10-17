## Capstone Project Final Report for specialized Master in Business Analytics (sMBA) - 2019
## Project Title
## WOSU Public Media Donor Database Analysis and Segmentation
 
This project provides business insights of first time donors, by applying Data wrangling, Descriptive (networks, geo-visualizations and histograms), Predictive and Prescriptive analysis for prospective Donor database expansion for WOSU Public media. 

WOSU is a public media enterprise serving Central Ohio and has consistently excelled in adding value and credibility. First time donors are a complement to sustained donors and additional planned gift support. Advanced statistical analysis identified opportunities to strengthen the basis of first-time donations:  
   a. for campaign goals 
 	 b. saving costs 
 	 c. increase donor conversions
  


## Through process and methods:

### 1.	Analyzing and Identifying meaningful and redundant variables

### 2.	Data wrangling   
a. Formatting the fields - use separate, unite, fix date field,    
b. Solicitation source -mutate to root word as categorical variable example ‘heard in radio’  to radio.  
c. Split Donor name as first name and last name  to link Event file and Original Gift Source.   
d. Augment to create Gender field. Use gender R package.   
e. Identify Organizations with key words as company, group, corporation, foundation, organization, campaign , firm, establishment, agency, office, enterprise, operation, institution, venture, undertaking, practice, society, league, club, network etc. And keep the set of observations as a separate file.   
f. State variable has data that spans across many states in US and territories . Ohio is the exceptional contributor so  will consider separately for analysis from the rest of states.  Added additional field of Regions and Divisions as a categorical variable.   
g. 22 Event text file has to be combined into one file with variables as First Name, Last name, Event month, Event year, Event day , Event name and Original Gift Source(root word).    
h. Check for Null Values.    
i. Merge the value “Additional Gift” from variable Orig_Gift_Pledge_type into variable Solicitaion_type.    


### 3.Exploratory data analysis both  univariate and bivariate.  
a. Use geo Spatial files to determine spread  of donors  across counter.    
b. Use network visualization  betweenness centrality for nodes as city names and Original gift source. The nodes at the critical junction has highest score.    
c. Compared the retention rate of donors based on Solicitation method.   
d. Determine the cost rate of ‘thank you gifts’ and the trend in years and months and the retention rate.    
e. See trends of event attendees over the years and months.    


### 4.	Statistical Significance.     
a. Use multinomial regression to regress the Mode of payment to Original Gift source.       
b. Use multinomial regression to regress Solicitation Method on Original Gift source.  


### 5.	 Predictive Analysis   
Predict the donantion amount with independent variables as Gift month, gift year, gender, various gift sources like radio, tv, acquisition, mail , special opportunity, showcase, passport, web, open ask, annual fund, cba ad otwhite, various Solicitaion methods like auto ren, email, other, online, telemarketing, renewal, gift has premium, mode of payment, account status.    
The data was split into training and test set.   
The algorithm was trained on the training set for regression tree, random forest, gradient boost and neural netwok models.   
The respective trained model was tested with Test data and the R2 was evaluated.    



### 6.	Prescriptive analysis
a.	In the year 2016 , WOSU started the Passport.  as a new member benefit with many privileges for donations of at least $60.00 or more.    
So here I am trying to see the difference in donation  between 2 periods with the treatment as Passport  being introduced.   
And the Differences-in-Differences method regression shows a positive impact with a lift of 18% in donations which is the causal effect.   

b.	Conjoint analysis - 
Conjoint survey helps in discovering the unmet needs or probe into the downstream  effect of  realization of donations.
Created  a sample of Conjoint Survey with Attributes and levels. A typical decision task that an individual gets for survey. Answers to these  can help in adding more meaningful variables and to know how people value these different attributes  and improve program content and thus increase  their engagement  and in turn donor conversion.       
 
  
##  Author
   Shyni David  
  
  
##  Acknowledgements
  Prof.  Waleed Muhanna, Ph.D. Fisher College of Business, The Ohio State University  
  Prof. Greg Allenby, Ph.D. Fisher College of Business, The Ohio State University  
  WOSU Public Media 
