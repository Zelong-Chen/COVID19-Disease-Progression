# COVID19-Disease-Progression

## Abstract 
In this project we look to compare the disease progression of the COVID-19 Coronavirus in the state of California under different operating assumptions. We want to analyze the effectiveness of the implementations put in place by California state officials that are aimed to lower the spread of the Coronavirus and “flatten the curve”. We will be focusing on the analysis of the Stay-At-Home Order and Coronavirus Testing / Contact Tracing. The Stay-At-Home Order was implemented to encourage citizens to remain at home to lower the number of unnecessary social contacts between individuals in order to reduce the spread of the virus. Coronavirus Testing / Contact Tracing was used to detect asymptomatic carriers and any individuals in contact with the carriers, in order to place them into quarantine to prevent further spread of the virus to the general population. This project will look to study both of these implementations separately first to analyze each of their effectiveness. Then combining both implementations to compare the overall effects of these interventions under different operating conditions versus a baseline of the disease progression without any interventions.

## Model  
We aim to model the COVID-19 virus as an infectious disease under the SEIR (Susceptible, Exposed, Infectious, Recovered) Compartmental Model. In addition to these four compartments, we will also add in a Death compartment to simulate and analyze the death tolls due to the Coronavirus. Using this model we will model the disease progression under different operating conditions such as with Stay-At-Home Order and/or Coronavirus Testing / Contact Tracing. We will use the program Anylogic to perform system dynamics modeling that will simulate the spread of the COVID-19 virus as it spreads through the population of California. Details of the models are explained in later sections. We hope to analyze the effectiveness of these implementations put in place by the state officials to lower the spread of the Coronavirus and “flatten the curve”. For this analysis, we will not be studying the possibility of reinfection after recovering from the virus as there is not enough data currently to support this. Thus, this project will simulate the disease progression of the disease from Susceptible to Exposed to Infectious to either Recovered / Death.

### SEIR-D Baseline
![alt text](https://github.com/Zelong-Chen/COVID19-Disease-Progression/blob/master/images/seird.PNG)

### SEIR-D + Stay-At-Home Order
![alt text](https://github.com/Zelong-Chen/COVID19-Disease-Progression/blob/master/images/seird_stay.PNG)

### SEIR-D + Testing / Contact Tracing
![alt text](https://github.com/Zelong-Chen/COVID19-Disease-Progression/blob/master/images/seird_testing.PNG)

### All-in-One Model
![alt text](https://github.com/Zelong-Chen/COVID19-Disease-Progression/blob/master/images/seird_allinone.PNG)

## Results
![alt text](https://github.com/Zelong-Chen/COVID19-Disease-Progression/blob/master/images/result1.PNG)  
From the results above, the blue curve represents the baseline of the disease progression of COVID-19 without any interventions. 70% represents the average / current mobility trend of California under Stay-At-Home Order. We can see that the effects of the Stay-At-Home order at 70% mobility is able to reduce the infectious population by -16.42%. At 40% mobility, which represents California’s best efforts and lowest mobility trend during the Stay-At-Home order was able to reduce the infectious population by -49.59%. It is interesting to note that with very strict lockdown intervention (i.e. 10% mobility), similar to the ones that occurred in China, the infectious population will not grow exponentially at all. Thus, showing that Stay-At-Home order is an essential intervention that effectively decreases the spread of the Coronavirus and helps tremendously in “flattening the curve.” In addition to decreasing the spread of Coronavirus, lower mobility trends also delays the peak of infection. Which will allow the state of California to have additional time to prepare the necessary resources such as hospital beds, invasive ventilators, and personal protection equipment to combat the large influx of patients during the peak of infection.  

Results from the simulation of SEIR-D + Contact Tracing/Testing is shown above. When compared to the baseline, we can see that the current capacity of testing available in California (16,000 and 25,000 in May) did have an effect on lowering the peak of the curve. However the respective percent change of peak infectious patients are -6.58% and -10.07%. Although this is a good indication of the effects brought on by Contact Tracing/Testing to lower the spread of the virus, we can see that California is still behind in providing the necessary testing kits. The result suggests that we need to reach the capacity of 70,000 to have an large impact on lowering the spread of the Coronavirus, with a -25.2% decrease in the number of infections. If combined with the Stay-At-Home Order, it can lead to reopening the state sooner.

## All-in-One Results
![alt text](https://github.com/Zelong-Chen/COVID19-Disease-Progression/blob/master/images/result2.PNG)  
Results of the number of infectious and death from the All-in-One model is shown above. All-in-One includes both interventions of Stay-At-Home Order and Contact Tracing / Testing with different permutation of parameters. The orange curve above represents the current situation in California with Stay-At-Home Order reducing mobility trends to about 70% and COVID-19 capacity of 16,000 tests per day.  When compared to the blue baseline model with no interventions put in place, the current situation decreases the peak infection by -23.16% and total death by -1.59%. These results show that we are making good progress in lowering the spread of Coronavirus through these interventions. But as mentioned before the most effective way to lower the spread is to enforce a strict Stay-At-Home Order to lower the mobility trend of citizens, which in terms will lower the spread of the virus by a significant amount. For example, with a mobility trend of 40% and test capacity of 16,000, can decrease the peak infection by -55.67% and total death by -10.73%.

## Files
### Presentation:
Presentation 4 (COVID-19).pdf  
### Report: 
Project 4 Report(COVID-19).pdf  
### Baseline (w/o Interventions): 
SEIR-D _ Simulation.mp4  
### Stay-At-Home Order:   
SEIR_D_stay _ Simulation.mp4  
### Testing/Contact Tracing:   
SEIR_testing _ Simulation.mp4  
### All-in-One Model:   
SEIR_all_in_one _ Simulation.mp4   
