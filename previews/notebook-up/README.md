# Connect to Jupyter Notebook with "az ml notebook up" in CLI v2 (Private Preview)

## Overview 

ML professionals are used to typing `jupyter notebook` to start their ML data & training workflows.  With `az ml notebook up`, Azure ML users can now move their code & notebooks to the cloud in one CLI command, and start using cloud data and compute in their workflows. 

## Prerequisite 

* Azure subscription. If you don't have an Azure subscription, , sign up to try the [free or paid version of Azure Machine Learning](https://azure.microsoft.com/free/) today.

* Azure CLI and ML extension. For more information, see [Install, set up, and use the CLI (v2) (preview)](how-to-configure-cli.md). 

* Existing compute resource in your workspace. Learn how to [create an Azure Machine Learning compute cluster](https://docs.microsoft.com/azure/machine-learning/how-to-create-attach-compute-cluster?tabs=python). 


## Get started 

Now you have installed and set up the CLI v2, you can use the `az ml notebook up` for your model development. 

### Create compute in CLI

You can create an Azure Machine Learning compute cluster from the command line. For instance, the following commands will create one cluster named `cpu-cluster`.
```dotnetcli
az ml compute create -n cpu-cluster --type amlcompute --min-instances 0 --max-instances 10 
```
Note that you are not charged for compute at this point as `cpu-cluster` will remain at 0 nodes until a job is submitted. Learn more about how to [manage and optimize cost for AmlCompute](how-to-manage-optimize-cost.md#use-azure-machine-learning-compute-cluster-amlcompute).

The following example in this article use `cpu-cluster`. Adjust these as needed to the name of your cluster.

Use `az ml compute create -h` for more details on compute create options.

### Create a  new notebook 

## Coming soon

* Support distributed training with multi-nodes compute.
* Support clusterless compute as default compute to start with in case you don't have an existing compute. 
* Connect to VS Code using `az ml vscode up`. 
