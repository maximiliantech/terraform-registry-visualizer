# Terraform Registry Visualizer
## Motivation
[Terraform by HashiCorp][terraform_url] is an Open Source tool to orchestrate infrastructure on any cloud. It uses the Infrastructure as Code (IaC) approach to simply define resources and track the states of the provisioned infrastructure.
To make this possible Terraform uses its own concepts of Providers and Modules.
Providers and Modules from different vendors are published in the [Terraform Registry][terraform_registry_url].
This tool visualizes specific metrics of three Providers ([AWS][terraform_aws], [Azure][terraform_azure] and [GCP][terraform_gcp]) from the [Terraform Registry][terraform_registry_url] and from GitHub. 

## Implementation
Mostly, the code of Providers and Modules are available Open Source on GitHub.
The following list shows which metrics are visualized -> and their origin:
- Download metrics of each Provider -> Terraform Registry Provider [AWS][terraform_aws], [Azure][terraform_azure] and [GCP][terraform_gcp]
- Number of Modules available for each Provider -> [Terraform Registry][terraform_registry_url]
- Number of Stars for each Provider -> GitHub Repository [AWS][github_aws], [Azure][github_azure] and [GCP][github_gcp]
- Number of Open Issues for each Provider -> GitHub Repository [AWS][github_aws], [Azure][github_azure] and [GCP][github_gcp]
- Number of Forks for each Provider -> GitHub Repository [AWS][github_aws], [Azure][github_azure] and [GCP][github_gcp]

UPCOMING: What's interesting to visualize:
- Number of Contributors for each Provider -> GitHub Repository [AWS][github_aws], [Azure][github_azure] and [GCP][github_gcp]

<!-- Links -->
[terraform_url]: https://www.terraform.io/
[terraform_registry_url]: https://registry.terraform.io
[terraform_registry_api_docs]: https://www.terraform.io/registry/api-docs
[terraform_aws]: https://registry.terraform.io/providers/hashicorp/aws/latest
[terraform_azure]: https://registry.terraform.io/providers/hashicorp/azurerm/latest
[terraform_gcp]: https://registry.terraform.io/providers/hashicorp/google/latest
[github_aws]: https://github.com/hashicorp/terraform-provider-aws
[github_azure]: https://github.com/hashicorp/terraform-provider-azurerm
[github_gcp]: https://github.com/hashicorp/terraform-provider-google