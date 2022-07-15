# Terraform Registry Visualizer
## Motivation
[Terraform by HashiCorp](https://www.terraform.io) is a great tool to orchestrate infrastructure on any cloud. They use the Infrastructure as Code (IaC) approach to simply define resources and track the states of the provisioned infrastructure.
To make this possible they use their own concepts of Providers and Modules which are published in the [Terraform Registry](https://registry.terraform.io).
This little tool showcases the three biggest Providers ([AWS](https://registry.terraform.io/providers/hashicorp/aws/latest), [Azure](https://registry.terraform.io/providers/hashicorp/azurerm/latest) and [GCP](https://registry.terraform.io/providers/hashicorp/google/latest)) in the [Terraform Registry](https://registry.terraform.io). 

## Implementation
This tool uses the official [Terraform Registry HTTP API](https://www.terraform.io/registry/api-docs) to get metrics like number of downloads etc. 