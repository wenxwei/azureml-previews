# Connect to Jupyter Notebook with "az ml notebook up" in 2.0 CLI (Private Preview)

## Overview 

ML professionals are used to typing `jupyter notebook` to start their ML data & training workflows.  With `az ml notebook up`, Azure ML users can now move their code & notebooks to the cloud in one CLI command, and start using cloud data and compute in their workflows. 

## Prerequisite 

* To use Azure machine learning, you must have an Azure subscription. If you don't have an Azure subscription, create a free account before you begin. Try the [free or paid version of Azure Machine Learning](https://azure.microsoft.com/free/) today.

* You must install and configure the Azure CLI and ML extension. For more information, see [Install, set up, and use the CLI (v2) (preview)](how-to-configure-cli.md). 

* You must have an Azure Resource group, in which you (or the service principal you use) need to have `Contributor` access. You'll have such a resource group if you configured your ML extension per the above article. 

* You must have an Azure Machine Learning workspace. You'll have such a workspace if you configured your ML extension per the above article.

* You must have an existing compute resource in your workspace 


## Get started 




## Coming soon

* Support distributed training with multi-nodes compute.
* Support clusterless compute as default compute to start with in case you don't have an existing compute. 
* Connect to VS Code using `az ml vscode up`. 
