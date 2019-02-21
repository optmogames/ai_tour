### House Prices  Prediction with Deep Learning on Azure Machine Learning service

#### Instructions to run this tutorial. Here we also include links for more information about the key concepts behind Azure ML service:

1. Follow the instructions [here](https://docs.microsoft.com/en-us/azure/machine-learning/service/quickstart-create-workspace-with-python) until the step named "Install the SDK" to create a local Python environment where you will install the Azure Machine Learning service SDK.

2. (Optional) Run the **DL_Regression.ipynb** notebook. This is a standalone notebook (not dependent on the Azure ML service SDK). It will train a regression model using Deep Learning techniques. The code in this notebook is the basis for the [Training Script](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-azure-machine-learning-architecture#training-script) to be used by the following notebooks. It is intended to explain how the dataset is prepared and how the deep learning model is defined and trained, using the PyTorch Deep Learning framework.

3. Run the **Azure ML/Configuration.ipynb** notebook. This will create a [Workspace](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-azure-machine-learning-architecture#workspace) and a [Compute Target](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-azure-machine-learning-architecture#compute-target) to train your models on.

4. Run the **Azure ML/Train_Model.ipynb** notebook. This will create an [Experiment](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-azure-machine-learning-architecture#experiment) for model training. As part of that, you will create a configuration for accessing a shared [Datastore](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-azure-machine-learning-architecture#datastore) and also a [Pytorch Estimator](https://docs.microsoft.com/en-us/azure/machine-learning/service/how-to-train-pytorch) that defines the environment for your  Deep Learning model training.

5. Run the **Azure ML/Train_Model_Hyperdrive.ipynb** notebook. It is similar to the notebook above, but it encapsulates the PyTorch Estimator into a [Hyperdrive](https://docs.microsoft.com/en-us/azure/machine-learning/service/how-to-tune-hyperparameters) object for automatic model hyperparameter tuning. You can then get information from your [Run](https://docs.microsoft.com/en-us/azure/machine-learning/service/concept-azure-machine-learning-architecture#run) job to see which combination of hyperparameters gives you the best model according to your [primary metric](https://docs.microsoft.com/en-us/azure/machine-learning/service/how-to-tune-hyperparameters#specify-primary-metric) objective.

#### To learn more:

[Azure ML service notebooks on GitHub](https://github.com/Azure/MachineLearningNotebooks)

[Microsoft Learn AI - Anomaly Detection & Predictive Maintenance](https://github.com/Azure/LearnAI-ADPM)

[Microsoft Learn AI - Custom AI Airlift](https://github.com/Azure/LearnAI-CustomAI-Airlift)
