# ucb-aiml-capstone





~~~ 
~~~ PROBLEM STATEMENT AND CONTEXT
~~~ 

In an electrical engergy market, it is the role and responsibility of an Independent 
System Operator (ISO) to manage that market.

There are numerous producers and consumers of electrical energy participating in a 
market.  Matching the constantly and dynamically changing balance point of supply 
and demand is a continual ongoing effort.  The general problem is to do this as 
efficiently and effectively as possible under conditions of uncertainty.

There are nine ISOs in North America, of which two examples are are the California 
Independent System Operator (CAISO) and New York Independent System Operator (NYISO).
CAISO data is examined in the course of this project. 

In an electrical market, the consumer demand is ultimately expressed as "Total Load" in 
the system. The various suppliers of electricity are categorized by fuel type (e.g. Coal, 
Hydro, Natural Gas, Nuclear, etc).  Collectively this is known as "Fuel Mix".  At any 
moment, The Total Load is matched and balanced with the The Fuel Mix. These are the data 
sets used in this capstone project. The values in each data set are expressed numerically 
in megawatt hours (MWh).

In recent years, Solar and Wind renewable energy sources have come into widespread use 
with increasing share of the fuel mix when they are available.  One problem with Solar and 
Wind is that the electricity they produce has to be used immediately or stored somehow, 
otherwise it is lost.  This is particularly predominant for the CAISO who have been market 
leaders for the innovation and adoption of Solar and Wind.

By subtracting Solar and Wind from the Total Load, a new line can be drawn on charts 
representing the total production and consumption.  This line is known as The Duck Curve.
The Duck Curve represents the amount of energy which needs to be produced by energy 
sources other than Solar and Wind in order to meet demand. 

Several negative side effects occur because the Duck Curve phenomena increases the total 
volitility of demand for non-Solar & non-Wind sources. Most noteably, the daily 
variablility of production is more extreme for the non-renewables, which puts greater 
strain on equipment and workers.  Unforeseen changes can cascade throughout the system, 
and increased variability can severely impact electricity generation, transmission and 
distribution as well as supply chain and pricing and other effects. 

This is the general situation and the problem.    

One solution to help increase efficency and manage the systems more effectively, is to 
create reliable and accurate forecasts of The Total Load and The Duck Curve.  Doing so 
helps managers and operators plan ahead for likely scenarios, and thus be able to prepare 
ahead of time to meet increased demand or cover shortfalls in Solar and Wind.

Forecasting is a complex and multifaceted activity. 

A first level of forecasting is to seperate out the underlying trends for Total Load
and Fuel Mix.  That is the aim of this capstone project.  This is done by isolating the 
trend via Seasonal Decomposition and seperating the trend from the seasonality and residue 
of the Total Load and Fuel Mix timeseries. 

More advanced solutions would be to understand and refine the methods by 
creating increasingly sophisticated predictions such as forecasting the entire 
timeseries for Total Load and Fuel Mix. 

Further forecasting refinements could be to include information from other data 
sets such as: 

    weather forecasting data,
    data from smart grid sensors, and
    commodity pricing (i.e. oil and gas, coal etc.).






~~~
~~~ OVERVIEW 
~~~


The message below is the initial proposal submitted earlier in the course to 
establish the subject and objective of the Capstone Project (see below). 

For the Capstone 1 submission, the items listed as [p1] [p2] [p3] (see below) were 
able to be addressed by writing the initial code and results.  These were further 
refined, extended, and made more robust. 


~~~
~~~ INITIAL PROPOSAL 
~~~

Hi Aravind, 

It was nice meeting you on the call earlier today.  

As we discussed, I'm thinking to proceed with the Electrical Power Grid Timeseries proposal 
for my capstone. Specifically I'm interested to characterize the supply & demand aspects 
of as illustrated by "The Duck Curve". I want to understand seasonality, and then do 
forecasting and other predictive analytics. My objective is to do a more thorough study of 
the material presented in module 10, and then go beyond that material to do analytics using 
additional and recent tools techniques and methods.

I see this as a multi phase effort according to following broad outline. I see [p1] - [p4]
as being achievable by the holidays. And [p5] or [p6] as nice-to-have follow on additional
work if there is time and capacity available to complete prior to the end of the program. 
The outline is:

    [p1] data gathering and collection,
    [p2] data organization and cleaning,
    [p3] basic analysis (i.e. use methods in mod 10),
    [p4] intermediate analysis (i.e. SARIMA/SARIMAX beyond mod 10),
    [p5] advanced analysis (i.e. work on actual industry problems), and
    [p6] comprehensive advanced analysis (i.e. ISO intermarket comparsions).

where phases [p1] - [p3] is the initial goal, and would form the foundataion for 
any further work if there is time. The following EMS dataset contains over five years 
historical timeseries data at the hourly grainularity for the CASIO component organizations 

https://www.caiso.com/library/historical-ems-hourly-load
Historical EMS hourly load 



Extending beyond mod 10 [p4] would utilize other available methods and techniques (e.g. SARIMA 
& SARIMAX).  Once the basics are accomplished, I would be very interested to go deeper into 
the use of SARIMA as you had suggested as well as analyze the impact of exogenous factors such 
as weather or fire using SARIMAX.


[p5] would be to get into actual industry research and problem solving. 

An examples problem can be found here:

https://www.rtoinsider.com/73329-transfer-limitations-during-q3-significantly-impact-weim-dmm-reports/
DMM: CAISO Transfer Limitations During Q3 Heat Waves Led to Price Disparities


There are nine ISOs in North America, [p6] and it would be interesting to do intermarket cross comparison 
study among and between these different markets.


Thanks and looking forward to working with you on this project. 


All the Best,
Mike Jones





