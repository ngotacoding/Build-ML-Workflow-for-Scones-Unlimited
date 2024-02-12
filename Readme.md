## Build ML Workflow for Scones Unlimited

This is the final project of the AWS Machine Learning Fundamentals Nanodegree by Udacity

### Project Overview
The project involves developing an image classification model to enhance the operations of Scones Unlimited, a scone delivery logistics company. The goal is to build a scalable and robust image classification model using AWS SageMaker. The model will differentiate between bicycles and motorcycles, enabling Scones Unlimited to optimize their delivery routing by assigning appropriate orders to drivers based on their vehicle type. The model will be deployed using AWS SageMaker, with supporting services built using AWS Lambda functions and Step Functions. 

## Dataset
The CIFAR dataset is utilized, comprising images of various objects, including vehicles like bicycles and motorcycles. This dataset serves as the foundation for training the image classification model, enabling accurate differentiation between different vehicle types to optimize delivery routing at Scones Unlimited.

### Project Steps Overview

1. **Data Staging**: Extract, transform, and load dataset to simulate image classification challenges faced by Scones Unlimited.
2. **Model Training and Deployment**: Train the image classification model using AWS SageMaker's built-in algorithm, deploy it, and configure Model Monitor for tracking.
3. **Lambdas and Step Function Workflow**: Develop and deploy three Lambda functions to generate data, perform image classification, and filter low-confidence inferences. Use Step Functions to orchestrate these functions.
4. **Testing and Evaluation**: Perform invocations of the Step function using test dataset to validate workflow behavior. Use SageMaker Model Monitor data to create visualizations for model monitoring.

## Project Structure
```bash
Build ML Workflow for Scones Unlimited/
├── lambda.py                    # Python script containing code for Lambda functions
├── main.html                    # HTML file for main notebook display
├── main.ipynb                   # Main Jupyter notebook for the project
├── README.md                    # Project overview and instructions
├── Step Function.json           # JSON file containing Step Function configuration
├── Step Functions.png           # Screenshot of the Step Functions visual editor
└── success step function.png    # Screenshot of the successful Step Function execution
```

## Development Environment Setup

The project notebook is run on AWS sagemaker with Python 3 (Data Science) kernel.
The recommended instance type is ml.t3.medium instance.