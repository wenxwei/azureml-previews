# Azure Machine Learning previews

Welcome to the Azure Machine Learning previews repository!

## Prerequisites

1. An Azure subscription. If you don't have an Azure subscription, [create a free account](https://aka.ms/AMLFree) before you begin.
2. A terminal with the [Azure CLI installed](https://docs.microsoft.com/cli/azure/install-azure-cli).
3. Install and set up the 2.0 machine learning extension:

    ```terminal
    az extension add --source https://azuremlsdktestpypi.blob.core.windows.net/wheels/sdk-cli-v2-public/ml-2.0.0a1-py3-none-any.whl --pip-extra-index-urls https://azuremlsdktestpypi.azureedge.net/sdk-cli-v2-public -y
    ```

## Public previews (MSFT internal)

Public preview examples can be found at https://github.com/Azure/azureml-examples/tree/main/cli. Documentation is currently available for MSFT internal. If enrolled in the private preview, reach out to your rep for a copy of the docs.

Installation and set up:

- [Install, set up, and use the 2.0 CLI](https://review.docs.microsoft.com/azure/machine-learning/how-to-configure-cli?branch=release-build-2021-azureml)
    - **Note:** `az extension add -n ml` will not work yet, see above for installation
- [Set up the VSCode extension](https://review.docs.microsoft.com/azure/machine-learning/how-to-setup-vs-code?branch=release-build-2021-azureml)

Train models (create jobs):

- [Train models (create jobs) with the 2.0 CLI](https://review.docs.microsoft.com/azure/machine-learning/how-to-train-cli?branch=release-build-2021-azureml) 

Endpoints:

- [What are Azure Machine Learning endpoints?](https://review.docs.microsoft.com/azure/machine-learning/concept-endpoints?branch=release-build-2021-azureml)
- [Deploy and score a machine learning model with a managed online endpoint](https://review.docs.microsoft.com/azure/machine-learning/how-to-deploy-managed-online-endpoints?branch=release-build-2021-azureml)
- [Safe rollout for online endpoints](https://review.docs.microsoft.com/azure/machine-learning/how-to-safely-rollout-managed-endpoints?branch=release-build-2021-azureml)
- [Use managed online endpoints in the studio](https://review.docs.microsoft.com/azure/machine-learning/how-to-use-managed-online-endpoint-studio?branch=release-build-2021-azureml) 
- [Viewing costs for managed online endpoints](https://review.docs.microsoft.com/azure/machine-learning/how-to-view-online-endpoints-costs?branch=release-build-2021-azureml)
- [Managed online endpoints SKU list](https://review.docs.microsoft.com/azure/machine-learning/reference-managed-online-endpoints-vm-sku-list?branch=release-build-2021-azureml) 
- [Monitoring managed online endpoints](https://review.docs.microsoft.com/azure/machine-learning/how-to-monitor-online-endpoints?branch=release-build-2021-azureml)
- [Troubleshooting managed online endpoints](https://review.docs.microsoft.com/azure/machine-learning/how-to-troubleshoot-managed-online-endpoints?branch=release-build-2021-azureml)
- [Batch scoring with batch endpoints](https://review.docs.microsoft.com/azure/machine-learning/how-to-use-batch-endpoint?branch=release-build-2021-azureml)
- [Troubleshooting batch endpoints](https://review.docs.microsoft.com/azure/machine-learning/how-to-troubleshoot-batch-endpoints?branch=release-build-2021-azureml)

## Private previews

Pipelines:

- [Introduction and set up](previews/pipelines)

AutoML:

- [Introduction and set up](https://github.com/Azure/AutoML-vNext-Preview)

## Contents

|directory|description|
|-|-|
|`.github`|GitHub-specific files like Actions workflow definitions and issue templates|
|`previews`|Self-contained directories of private previews|

## Contributing

We welcome contributions and suggestions! Please see the [contributing guidelines](CONTRIBUTING.md) for details.

## Code of Conduct

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). Please see the [code of conduct](CODE_OF_CONDUCT.md) for details.

