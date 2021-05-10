# Why and When to Employ MLOPS

## Data Scientists' Pain Point

### Currents Challenges Datascients facing

* operationalizing models and making them availalbe in production is difficult

    + Keep track of the meaning model 
    + Reproducibility of model
    + Model need to be update regular basis as new data comes in
    + Examine (monitoring) machine learning project (time, resources)

* solutions to this MLOps

## Machine Learning Lifecycle

* MLOps is a lifecycle management discipline for machine learning

### MLOps Concept
* Continuous Integration (CI)
    - Test automatically to check the application whenever new commits are integrated into the main branch
    
* continuous Delivery (CD)
    - Buiding, testing in releasing software in short cycle
    
* Continuous Training (CT)
    - Process of monitoring, measuring, retraining and serving the models

### Technical dept

* developing and deploying in ML system can be relatively fast and cheap, but maintaining over time can be difficult and expensive
    
    + Multi-functional teams
        - teams with data scientists and ml egineers, ... etc
    + Experimental nature
        - constantly try new approaches with the data, models, and parameter configuration
    + Testing complexity
        - keep track of what worked and what didn't in maintaining reproducibility while maximising causerie usability
    + Deployment complexity
        - deploy multi-step pipline to retrain and deploy the model
    + model decay
        * keep track of summary statistics of the data and monitor online performances

### MLOps vs DevOps

| DevOps                                             | MLOps                                                         |
|:--------------------------------------------------:|:-------------------------------------------------------------:|
| Test and validate code and components              | Also test and validate data, data schemas, and models         |
| Focus on a single software package or service      | Also consider the whole system: the ML training pipeline      |
| Deploy code and move to the next task              | Constantly, retrain, and serve the model                      |


## MLOps Architecture and Tensorflow Extended Components

### Phases of a machine learning project

* Discovery Phase
    - Define business use cases (1)
    - Data exploration (2)

* Development Phase
    - Data exploration (2)
    - Select algorithm (3)
    - Data pipeline and feature engineering (4)
    - Build ML model (5)
    - Evaluate (6)
    - Present result (7)

* Deployment Phase
    - Plan for deployment (8)
    - Operationalize model (9)
    - Monitor model (10)

### The level of automation defines the maturity of the ML process

| Level 0                   | Level 1                      | Level 2                                      |
|:-------------------------:|:----------------------------:|:--------------------------------------------:|
|Build and deploy manually  | Automate the training phase  | Automated training validation, and deployment|
