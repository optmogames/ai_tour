### Heart Disease Prediction with Azure Machine Learning service

#### Instructions to run this tutorial. Here we also include links for more information about the key concepts behind Azure ML service:

1. Follow the instructions [here](https://docs.microsoft.com/en-us/azure/machine-learning/service/quickstart-create-workspace-with-python) until the step named "Install the SDK" to create a local Python environment where you will install the Azure Machine Learning service SDK.

2. Run the **Classification.ipynb** notebook. This is a standalone notebook (not dependent on the Azure ML service SDK). It will train and save a simple classification model to be further operationalized using Azure ML service model deploying capabilities.

3. Run the **Azure ML/Configuration.ipynb** notebook. This will create a [Workspace](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-azure-machine-learning-architecture#workspace) and a [Compute Target](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-azure-machine-learning-architecture#compute-target) to train your models on.

4. Run the **Azure ML/Deploy_Model.ipynb** notebook. This will create an [Image](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-azure-machine-learning-architecture#image) with a score script that uses your trained model for inference and a [Deployment](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-azure-machine-learning-architecture#deployment) environment from where your score script will be exposed as a web service.

5. Run the **Azure ML/Train_Model_AutoML.ipynb** notebook. This will create an [Experiment](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-azure-machine-learning-architecture#experiment) for model training with [Automated ML](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-automated-ml). As part of that, you will create a configuration for accessing a shared [Datastore](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-azure-machine-learning-architecture#datastore) and also a [Run Configuration](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-azure-machine-learning-architecture#run-configuration) that defines the environment for your model training. After automatically training several models with Automated ML, you can retrieve information and the execution pipeline from the best [Run](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-azure-machine-learning-architecture#run), as well as [Model Explainability](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-automated-ml#model-explainability).

6. Run the **Azure ML/Deploy_Model_AutoML.ipynb** notebook. This will create an Image with a score script that uses the best trained model retrieved from the Automated ML job for inference and a Deployment environment from where your score script will be exposed as a web service.

#### To learn more:

[Azure ML service notebooks on GitHub](https://github.com/Azure/MachineLearningNotebooks)

[Microsoft Learn AI - Anomaly Detection & Predictive Maintenance](https://github.com/Azure/LearnAI-ADPM)

[Microsoft Learn AI - Custom AI Airlift](https://github.com/Azure/LearnAI-CustomAI-Airlift)
