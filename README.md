# Terraform Registry Visualizer
## Motivation
[Terraform by HashiCorp](https://www.terraform.io) is an Open Source tool to orchestrate infrastructure on any cloud. They use the Infrastructure as Code (IaC) approach to simply define resources and track the states of the provisioned infrastructure.
To make this possible they use their own concepts of Providers and Modules.
Providers and Modules from different vendors are published in the [Terraform Registry](https://registry.terraform.io).
This little tool visualizes some metrics of three Providers ([AWS](https://registry.terraform.io/providers/hashicorp/aws/latest), [Azure](https://registry.terraform.io/providers/hashicorp/azurerm/latest) and [GCP](https://registry.terraform.io/providers/hashicorp/google/latest)) from the [Terraform Registry](https://registry.terraform.io) and from GitHub. 

## Implementation
This tool uses the official [Terraform Registry HTTP API](https://www.terraform.io/registry/api-docs) to get metrics like number of downloads etc. 