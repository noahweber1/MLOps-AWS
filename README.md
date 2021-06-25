# MLOps-AWS

This projects serves as an example of deploying MLOPs on AWS.

[Walkthrough of the project can be found on Youtube](https://www.youtube.com/watch?v=QImMWBdnEJY)

This project is a containerized auto-scaling ML application to predict medical expenditures hosted on AWS. 


# Architecture
![Architecture](https://raw.githubusercontent.com/joekrinke15/MLModelDeployment/master/MLFinalProject.png)



A more detailed written description of the project can be found [here](https://github.com/noahweber1/MLOps-AWS/raw/master/detailed_walkthrough.pdf).

# User Interface 
## Index Page

![Index](https://raw.githubusercontent.com/joekrinke15/MLModelDeployment/master/UI.PNG)

## Prediction Page
![Prediction](https://raw.githubusercontent.com/joekrinke15/MLModelDeployment/master/SampleOutput.PNG)
# Sample Web API Call

Here is a sample call to the API with the following parameters:

Age: 23

BMI: 25

Number of Children: 3

Sex: Male

Smoking Status: Yes

Region: Southwest

Host IP Address: 54.224.27.206

```
curl -v -H "Content-Type:application/json" -X POST -d "{\"age\":23, \"bmi\":25, \"children\":3, \"female\":0, \"male\":1, \"no\":1, \"yes\":0, \"northeast\":1, \"northwest\":0, \"southeast\":0, \"southwest\":0}" 54.224.27.206/:8080/predict
```

Here is the response:
```
{"prediction":[3284.857731772743]}
```
# Architecture
![Architecture](https://raw.githubusercontent.com/joekrinke15/MLModelDeployment/master/MLFinalProject.png)


This was inspired by Noah Gift.

Buy his book here https://learning.oreilly.com/library/view/practical-mlops/9781098103002/