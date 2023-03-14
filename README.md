# Azure DevOps Agent 

This repository contains Packer Code & Azure Pipelines to create a Shared Image inside an Azure Compute Gallery which can be used as an Azure DevOps Agent on either a Virtual Machine or Virtual Machine Scale Set.

This repository is a scaled down version of Microsoft [runner-images](https://github.com/actions/runner-images).

## Image Generation

A new image is automatically generated monthly to ensure the base image is up to date with the latest security patches. The image is tagged with the format **yyyyMMdd.0.0**.

## Adding New Software

Before merging any changes to the Packer directory, please ensure:

- Change are built and tested in a Dev/Sandbox environment from your local machine.
- New software has tests to check the installed software is as expected.
- Any documentation outlining software is updated.

Documentation on how to use Packer can be found [here](https://developer.hashicorp.com/packer/plugins/builders/azure/arm).

## Installed Software

For all installed software, please refer to documentation found [here](https://github.com/hmcts/azure-devops-packer/tree/master/images/linux/ubuntu2204.md).