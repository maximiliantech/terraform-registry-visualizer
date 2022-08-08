# Terraform Registry Visualizer
## Motivation
[Terraform by HashiCorp][terraform_url] is an Open Source tool to orchestrate infrastructure on any cloud. It uses the Infrastructure as Code (IaC) approach to simply define resources and track the states of the provisioned infrastructure.
To make this possible Terraform uses its own concepts of Providers and Modules.
Providers and Modules from different vendors are published in the [Terraform Registry][terraform_registry_url].
This tool visualizes specific metrics of three Providers ([AWS][terraform_aws], [Azurerm][terraform_azurerm] and [Google][terraform_google]) from the [Terraform Registry][terraform_registry_url] and from GitHub. 

## Implementation
Mostly, the code of Providers and Modules are available Open Source on GitHub.
Additionally, there is a [Terraform Registry HTTP API][terraform_registry_api_docs] that allows to discover the [Terraform Registry][terraform_registry_url].

The following list shows which metrics are visualized -> and their origin:
- Download metrics of each Provider -> Terraform Registry Provider [AWS][terraform_aws], [Azurerm][terraform_azurerm] and [Google][terraform_google]
- Number of Modules available for each Provider -> Terraform Registry Modules filtered by [AWS][terraform_modules_aws], [Azurerm][terraform_modules_azurerm] and [Google][terraform_modules_google]
- Number of Stars for each Provider -> GitHub Repository of [AWS][github_aws], [Azurerm][github_azurerm] and [Google][github_google]
- Number of Open Issues for each Provider -> GitHub Repository of [AWS][github_aws], [Azurerm][github_azurerm] and [Google][github_google]
- Number of Forks for each Provider -> GitHub Repository of [AWS][github_aws], [Azurerm][github_azurerm] and [Google][github_google]

UPCOMING: What's interesting to visualize:
- Number of Contributors for each Provider -> GitHub Repository of [AWS][github_aws], [Azurerm][github_azurerm] and [Google][github_google]

<!-- Links -->
[terraform_url]: https://www.terraform.io/
[terraform_registry_url]: https://registry.terraform.io
[terraform_registry_api_docs]: https://www.terraform.io/registry/api-docs
[terraform_aws]: https://registry.terraform.io/providers/hashicorp/aws/latest
[terraform_azurerm]: https://registry.terraform.io/providers/hashicorp/azurerm/latest
[terraform_google]: https://registry.terraform.io/providers/hashicorp/google/latest
[terraform_modules_aws]: https://registry.terraform.io/browse/modules?provider=aws
[terraform_modules_azurerm]: https://registry.terraform.io/browse/modules?provider=azurerm
[terraform_modules_google]: https://registry.terraform.io/browse/modules?provider=google
[github_aws]: https://github.com/hashicorp/terraform-provider-aws
[github_azurerm]: https://github.com/hashicorp/terraform-provider-azurerm
[github_google]: https://github.com/hashicorp/terraform-provider-google