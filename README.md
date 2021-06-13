# Description of the project
Make sure you have installed Terraform, AWS CLI, and configured a default AWS CLI profile
# Configuration
Generate a personal access token **GitHub**

Make changes to `variables.tf`
```
variable "github_token" {}

variable "github_username" {
  default = "your_github_username"
}

variable "github_project_name" {
  default = "your_github_project_name"
}

variable "bucket_name" {
  default = "your_unique_s3_bucket_name"
}
```
# Deploy
```
cd deploy # change to deploy directory
terraform init # initialises Terraform
terraform apply # deploys AWS stack
terraform destroy # destroys AWS stack
```

When prompted for github_token, provide the value and hit Return
