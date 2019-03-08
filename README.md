# DataBricksIRISClassify
IRIS Classification on Azure Databricks using Tensor Flow

What is Azure Databricks?
Azure Databricks is an Apache Spark-based analytics platform optimized for the Microsoft Azure cloud services platform.

1.How to create an Azure Databricks Account?
https://docs.microsoft.com/en-us/azure/azure-databricks/quickstart-create-databricks-workspace-portal

2.Go Ahead create a ML Cluster, with or without GPUs - https://docs.azuredatabricks.net/user-guide/clusters/create.html#
Here I created a ML cluster without GPUs.

3.Remember to generate the access tokens - 
https://docs.azuredatabricks.net/api/latest/authentication.html#generate-a-token

4.Imported an IPython Notebook (IrisClassificationSimple.ipynb), which I had created using Jupyter.

5.Upload the training(iris_training.csv) and test(iris_test.csv) data into dbfs using the Data tab.

5.Attached the same to the MLCluster.

Boom! Same results much faster though.
Accuracy of - 96% with a loss of 0.05 and much much faster :)

PS: the only modification I had to do was making pandas read.csv work, gave a path not found error, use the path as follows
  /dbfs/FileStore/....
  









