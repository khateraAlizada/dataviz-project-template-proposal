# Data Visualization Project

## Data

The data I propose to visualize for my project is from https://www.cms.gov/Research-Statistics-Data-and-Systems/Statistics-Trends-and-Reports/NationalHealthExpendData/Age-and-Gender. Personal health care (PHC) for different services( 'Dental Services', 'Durable Medical Equipment', 'Home Health Care', 'Hospital Care', 'Nursing Care Facilities and Continuing Care Retirement Communities', 'Other Health Residential and Personal Care', 'Other Nondurable Medical Products', 'Other Professional Services', 'Physician and Clinical Services', 'Prescription Drugs', 'Total Personal Health Care', 'Service')and different sources of funding (private health insurance, Medicare, Medicaid, out-of-pocket, and all other payers and programs) is available for five age groups: 0-18, 19-44, 45-64, 65-84, and 85 and over, for different gender groups males and females and total for even years from 2002 through 2014.

Column name, description, type

payer (medicaid, private health insurance, total, out-of-pocket, etc), categorical
service( dental services, durable medical equipment, home health care, hospital care, nursing care facilities, Nursing Care Facilities and Continuing Care Retirement Communities, etc ), categorical
age group ( 0-18, 19-45, 46-65, 66-84 and 85 and up, total), ordinal
gender( male, female, total), categorical, 
year (2002 -2014), quantitative


## Prototypes

I’ve created a proof of concept visualization of this data. It's a scatter plot and it shows out of pocket prescription drug expenses for ages 19-44 from 2002 - 2014 for males, females and total (blue, yellow and red dots) population groups respectively. Between 2004 - 2008 per capital out of pocket prescription drug expenditure increased for all population groups.



[![image](https://user-images.githubusercontent.com/20228364/219963275-523207c5-4195-43f6-8ff0-4712e47f178a.png)](https://vizhub.com/khateraAlizada/f61c94f3d98840feb5b0f85af6823c21?file=scatterPlot.js)

## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:

 * As time increase total per capital health expenses will increase. 
 * As population age group increases, their health expenses will also increase.
 * What is the difference between males and females per capita health spending in a given year? Children (0-18)?
 * How does male children and female children total health care expenditure differ?
 * How does working-age (19-64) males and females per capita health spending differ?
 * What percentage of health care spending accounted for females 65 and older and what percentage of 65 and older population are females?
 

## Sketches
![sketchProposal](https://user-images.githubusercontent.com/20228364/219959375-a033fec8-33d8-460c-b4e5-a0589371d5f2.png)
The sketch display per capital private health insurance expenditure for males and females between ages of 0-18 years for hospital care. It is hypothetical data. It shows that hospital care expenses increased for each group over time. 

## Open Questions

I wanted to display the data from a specific population group. For example, displaying  health expenses for a given gender group, for a given service, for a given payer and a given age group over time. I achieved my goal to display what I wanted to display at the beginning of the project. In this report, I will display a step by step various visualizations that helped me in accomplishing the final goal. 

Initially I uploaded my data in github gist. 

[![originaldata](https://user-images.githubusercontent.com/20228364/234727162-69994048-317c-44f9-8365-36d6620378bc.png)](https://gist.githubusercontent.com/khateraAlizada/1ad0d265acbd1d202666ec610d998314/raw/b9200cf2b0ba3dc7fa8fc6b63fd93b80a1a7e6f7/healthCareCostGrowth.csv)
I made certain changes in my dataset to make it in the correct format. Initially the column names 2002 -2014 started with a number. I changed these column names because the column names should not start with numerical values. I added a y to make them start with a letter.
[![uploadinData](https://user-images.githubusercontent.com/20228364/234731159-2204acb8-665c-4c75-a532-ebf771c966a5.png)](https://vizhub.com/khateraAlizada/7ce463b8b74e437aad7141396ba72725)


To display a time series data. I created a year column instead of having separate column for each year. The year column includes all even years between 2002-2014. In addition, I created another column expenditure that stores health expenses estimates. [![reformated dataset](https://user-images.githubusercontent.com/20228364/234731582-e5853cd1-e683-4c5b-926d-d1bf5804186c.png)](https://gist.githubusercontent.com/khateraAlizada/2365f9474eab3f24f42ac5fbe3c18f08/raw/55d654aecbc83d67d25b55b3e2837fbfe349b23d/healthExpensesYear.csv)

The first data viz I created was a scatter plot. The y axis displays health expenses. The x axis displays year. The different colorr dots display gender column (male, female and total). Because there are many rows for each attributes of the gender column. The scatter plot was hard to understand. 

[![scatterplot](https://user-images.githubusercontent.com/20228364/234728700-15925525-a871-4705-a366-2a9a2b1e36ef.png)](https://vizhub.com/khateraAlizada/eefbd6bb9e054de9ba9fd58e3f142bf9?edit=files&file=scatterPlot.js)


