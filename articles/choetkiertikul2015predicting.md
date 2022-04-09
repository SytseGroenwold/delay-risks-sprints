# Predicting delays in software projects using networked classification
* source: https://github.com/jai2shukla/JIRA-Estimation-Prediction/blob/master/delayed%20issues/ASE2015/preprint_ASE2015.pdf
* https://scholar.googleusercontent.com/scholar.bib?q=info:Ub5-AJrabj4J:scholar.google.com/&output=citation&scisdr=CgXU7pQTELHQ9Z17JG0:AAGBfm0AAAAAYht9PG0-8IIaqnhIQmAVlBptRWQZ7d8w&scisig=AAGBfm0AAAAAYht9PKu1jjNhWJjgCOPHFIokkdsyadbI&scisf=4&ct=citation&cd=-1&hl=en

## Analysis
* a lot of recent proposals in addressing risk try to infer any risk from only the user story
* this paper aims to use the networked data (issues being related to each other) to improve upon these existing models
* the network data is sourced from the attritbutes of the user stories in the data both explicitly (direct relation) and implicitly (relation is inferred from other task information)
* example explicit: task B can only start after task A is done.
* exampe implicit: task F is to be done by developer A, but developer A is still working on task C, D and E (each of these can but doesn't have to be already marked delayed)
* after gathering this data, the model to predict the delay in the software project works as follows
* The local classifier uses the 15 non-relational (local) features from the user stories
* the relational classifier uses the task relations in the earlier defined task network to predict any delays
* collective inference allows them to make a predictions simulataneously for multiple related tasks. This means that if Task A is delayed and Task B is very much related to task A, it has a high chance of being delayed as well. 

## Research gaps


## Data