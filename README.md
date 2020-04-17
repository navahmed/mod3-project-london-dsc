
# Module 3 Project - Seattle Terry Stops Arrest Predictor

## Background - 

A Terry Stop allows the police in USA to detain an individual based on 'reasonable suspicion' of involvement in criminal activity. The legal standard for arrests and warrants in the United States is probable cause. Reasonable suspicion is less than probable cause, and is more like an "inchoate and unparticularized suspicion or 'hunch". Reasonable suspicion must be based on "specific and articulable facts", "taken together with rational inferences from those facts", and the suspicion must be associated with the specific individual.

Terry Stops originated from a landmark Supreme Court case in 1969, 'Terry vs Ohio.' A police officer in Cleveland, Ohio detained 3 men on the premise that they were behaving suspiciously. The officer believed that the men were preparing for armed robbery. The officer detained the men, and conducted a pat down search, and retrieved a fire arm. 2 of the men were convicted of carrying a concealed weapon. This case was appealed to the Supreme Court, with the convicted arguing that the weapon was found during an illegal search under the Fourth Amendment. The Fourth Amendment states "The right of the people to be secure in their persons, houses, papers, and effects, against unreasonable searches and seizures, shall not be violated, and no warrants shall issue, but upon probable cause, supported by oath or affirmation, and particularly describing the place to be searched, and the persons or things to be seized." The court found that the detention was admissible as the officer had reasonable suspicion which could be articulated - that the individuals detained could be armed and dangerous. 

## Project Objective - 

The objective of this project is to try to predict whether a Terry Stop will result in an arrest. The dataset that we will use for this is Terry Stop data from Seattle, Washington between 2015 until 2020. It is a binary classification problem, and using the data we will look to create a prediction model based on the avaiable data to determine whether an individual is arrested or not during a Terry Stop.

## Project Methodology -

As part of our Methodology, we used Logisitic Regression as our baseline model. We then used Grid Search CV in order to tune the hyperparameters and tried to improve the performance of the model. We also looked at K-Nearest Neighbours, Decision Trees and Random Forest learners to assess the ability of these models in predicting arrests. In each instance, we looked at using Grid Search CV in order to optimise the models.

We then selected the best performing learner and analysed the implications of this model.


## Key Findings - 

The best performing learner was the Logistic Regression after using hyperparameter tuning with Grid Search CV. Our findings suggest that Officer Age, Seattle Location and Officer Race appears to have an impact on whether or not an individual is arrested at a Terry Stop.

We then looked into prevalence of crime in Seattle, and worked out a threshold rate to use on our model. The threshold rate is quite low, 0.11. This is mainly due to the fact that the cost of crime and the amount spent on fighting crime was considered. To arrive at a more balanced threshold rate, we will need to consider other economic factors, especially those pertaining to True Negatives and False Positives.

## Workflow - 

The main body of work can be found in the notebook folder and the order sequence runs as follows

1) Data Cleaning

2) EDA and Visualisation

3) Feature Engineering and Modelling.

The CSV files used for this project are saved in the CSV folder.

### References -

https://catalog.data.gov/dataset/terry-stops
https://www.law.cornell.edu/constitution/fourth_amendment
https://en.wikipedia.org/wiki/Terry_stop
https://en.wikipedia.org/wiki/Reasonable_suspicion
