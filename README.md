This Terraform Template is intended to Automate and bringing up Zscaler GOV DEMO for ZPA setup on AWS in one touch mode.
It will bring up 2 app connectors and 2 webservers in single regions.

# Pre-requisites for using this template:

- **Terraform Install:** To Download & Install Terraform, refer Link "www.terraform.io/downloads.html"
- **Zscaler Images:** Image available and added in AWS in .ami format for:
  - App Connector



# Usage:

- Download all the files in PC where Terraform is installed. It is recommended that place all the files in folder as terraform will store the state file for this environment once it is applied.
- Go to the folder "versa_poc_he_auto_config_v1" where all the required files are placed.

- Use command `terraform init` to initialize. it will download necessary terraform plugins required to run this template.
- Then use command `terraform plan` to plan the deployment. It will show the plan regarding all the resources being provisioned as part of this template.
- At last use command `terraform apply` to apply this plan in action for deployment. It will start deploying all the resource on Azure.

The following figure illustrates the redundant (high availability) headend topology created by the Terraform template(s).

It will require below files to run it.


|____README.md
|____main.tf
|____output.tf
|____variable.tf
|____terraform.tfvars