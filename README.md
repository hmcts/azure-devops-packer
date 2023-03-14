# Azure DevOps Agent 

This repository contains Packer Code & Azure Pipelines to create a Shared Image inside an Azure Compute Gallery which can be used as an Azure DevOps Agent on either a Virtual Machine or Virtual Machine Scale Set.

This repository is a scaled down version of Microsoft [runner-images](https://github.com/actions/runner-images).

## Adding New Software

Before merging any changes to the Packer directory (for example adding new software), it is reccomended that any changes are built and tested in a Dev or Sandbox environment from your local machine. Please ensure any new software packages have tests that check they the software is installed as expected. Documentation on how to use Packer can be found [here](https://developer.hashicorp.com/packer/plugins/builders/azure/arm).

## Installed Software

For all installed software, please refer to documentation found [here](https://github.com/hmcts/azure-devops-packer/tree/master/images/linux/ubuntu2204.md).