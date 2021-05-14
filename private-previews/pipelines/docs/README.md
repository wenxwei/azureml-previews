### Setup instructions for Pipeline Job with Command Components preview

Pre-reqs:
1. AzureML Workspce with a compute cluster created. We strongly recommend using an existing test or sandbox Workspace or creating a new Workspace becuase the private preview bits can have bugs. DO NOT TRY THE PREVIEW ON A WORKSPACE WITH PRODUCTION ASSETS.
2. If you do not have the Azure CLI installed, follow the installation instructions at https://docs.microsoft.com/cli/azure/install-azure-cli. 2.15 is the minimum version your need. Check the version with `az version`. You can use Azure Cloud Shell which has Azure CLI pre-installed: https://docs.microsoft.com/en-us/azure/cloud-shell/quickstart

Steps:

1. Remove any previous extension installations

```
az extension remove -n ml; az extension remove -n azure-cli-ml
```

2. Install the preview AzureML extension.

```
az extension add --source https://azuremlsdktestpypi.blob.core.windows.net/wheels/sdk-cli-v2/ml-0.0.79-py3-none-any.whl --pip-extra-index-urls https://azuremlsdktestpypi.azureedge.net/sdk-cli-v2 -y
```

Check if the installation was successful with `az version`

3. Login with `az login`

4. Set your workspace defaults

```
az account set -s "<your_subscription_name_or_id>"

az config set defaults.workspace="<your_workspace>"
az config set defaults.location="<your_region>"
az config set defaults.group="<your_workspace_resource_group>"
```

5. Make sure your setup is working with either of the list commands: `az ml compute list`, `az ml jobs list`, or `az ml data list`

6. Enable private preview features. Linux/Bash: `export AZURE_ML_CLI_PRIVATE_FEATURES_ENABLED="true"`. Windows: `set AZURE_ML_CLI_PRIVATE_FEATURES_ENABLED=true`

7. Clone this samples repo: 

```
cd $HOME
mkdir repos
cd repos
git clone https://github.com/Azure/azureml-v2-preview
cd azureml-v2-preview/pipelines
```

### Known issues (to be fixed soon...)

1. New environments and datasets are created each time job is submitted even when a registered environment or dataset are specified. 
2. Cannot hard-code data or values in `component_job` in a `pipeline_job`. Need to map everything to `inputs` or `outputs` at the `pipeline_job` level.
3. Cannot skip mapping component input values that have defaults specified in the component definition.
4. Cannot use Designer UI to drag-n-drop Components and create Pipelines.
5. Input strings with spaces must use eacaped quotes. E.g. "\"hello python world\""

